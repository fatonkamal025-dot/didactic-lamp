# VidShare Troubleshooting Guide

Common issues and solutions.

## Frontend Issues

### "Cannot find module" errors

**Solution:**
```bash
rm -rf node_modules
npm install
```

### Blank screen on load

**Check:**
1. Is backend running on port 5000?
2. Are Firebase credentials in `.env.local`?
3. Check browser console for errors
4. Clear browser cache

### Videos not loading

**Solutions:**
1. Check if Firestore has data
2. Verify database rules
3. Check network tab in DevTools
4. Ensure video URLs are valid

### Authentication failing

**Check:**
1. Firebase project is created
2. Email/Password auth is enabled
3. Credentials are correct
4. Check Firebase console logs

## Backend Issues

### Port already in use

**Solution:**
```bash
# Find and kill process on port 5000
lsof -i :5000
kill -9 <PID>

# Or use different port
PORT=5001 npm run dev
```

### Firebase connection error

**Check:**
1. Service account key is valid
2. Environment variables are set correctly
3. Firebase project exists
4. Firestore database is created
5. Check Firebase console for errors

### Cloudinary upload failing

**Solutions:**
1. Verify Cloudinary credentials
2. Check API key and secret
3. Ensure cloud name is correct
4. Check file size limits
5. Check rate limits

### CORS errors

**Solution:** Update backend `.env`:
```
CLIENT_URL=http://localhost:5173
```

For production:
```
CLIENT_URL=https://yourdomain.com
```

## Database Issues

### Firestore rules blocking access

**Solution:** Update rules in Firebase Console:
```json
rules_version = '2';
service cloud.firestore {
  match /databases/{database}/documents {
    match /{document=**} {
      allow read, write: if request.auth != null;
    }
  }
}
```

### Data not persisting

**Check:**
1. Are writes actually happening?
2. Check Firestore console for data
3. Verify database rules allow writes
4. Check for errors in Firebase logs

## Performance Issues

### Slow video loading

**Solutions:**
1. Optimize video codec
2. Enable compression
3. Use CDN for videos
4. Implement lazy loading
5. Add pagination

### High API latency

**Solutions:**
1. Check database indexing
2. Optimize queries
3. Add caching
4. Check network connection
5. Monitor backend resources

## Development Issues

### Hot reload not working

**Solution:**
```bash
# Restart Vite dev server
npm run dev
```

### Tailwind styles not applying

**Check:**
1. Tailwind config includes correct paths
2. PostCSS is configured
3. CSS is imported in main.jsx
4. Try clearing cache:
```bash
rm -rf .next node_modules/.cache
npm run dev
```

### ESLint/Prettier conflicts

**Solution:**
```javascript
// .eslintrc.js
{
  "extends": ["eslint:recommended", "prettier"]
}
```

## Deployment Issues

### Build fails

**Try:**
```bash
npm run build
# Check build errors
npm run preview  # Preview build
```

### Environment variables not loading

**Check:**
1. Variable names are correct
2. Variables are set in deployment platform
3. Use correct prefix (`VITE_` for frontend)
4. Rebuild after changing variables

### Website not updating

**Solutions:**
1. Clear deployment cache
2. Force rebuild
3. Clear browser cache
4. Check CDN cache
5. Verify new version deployed

## Mobile Issues

### Touch events not working

**Check:**
1. Is touch event handler attached?
2. Check z-index conflicts
3. Verify viewport meta tag

### Responsive design broken

**Test:**
1. Mobile browsers
2. Different screen sizes
3. Orientation changes
4. Check CSS media queries

## Getting Help

### Check Logs

**Frontend:**
- Browser console (F12)
- Network tab
- Application tab

**Backend:**
- Server terminal output
- Node.js error stack traces
- Firebase Console logs

### Debug Steps

1. Reproduce the issue
2. Check console for errors
3. Check network requests
4. Verify credentials/config
5. Try simpler version of code
6. Check documentation

### Report Issues

Create GitHub issue with:
- Error message
- Steps to reproduce
- Screenshots
- Environment (OS, browser, etc.)
- Console logs

### Contact Support

- GitHub Issues: [Create issue](https://github.com/fatonkamal025-dot/didactic-lamp/issues)
- Email: support@vidshare.com

---

Most issues are configuration-related. Double-check:
1. Environment variables
2. Firebase setup
3. Credentials
4. API connectivity
5. Database rules

Still stuck? Ask on GitHub Discussions!
