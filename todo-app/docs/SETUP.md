# Todo App - Complete To-Do Application with Local Storage

A modern, feature-rich to-do list application built with React 18, Tailwind CSS, and browser's local storage.

## ✨ Features

### Core Functionality
- ✅ **Add todos** - Create new tasks instantly
- ✅ **Edit todos** - Modify existing tasks
- ✅ **Delete todos** - Remove unwanted tasks
- ✅ **Mark as complete** - Track finished tasks
- ✅ **Search** - Find todos by keyword
- ✅ **Filter** - View All, Active, or Completed todos

### Priority & Organization
- 🔴 **High Priority** - Urgent tasks
- 🟡 **Medium Priority** - Regular tasks
- 🟢 **Low Priority** - Less important tasks
- 📁 **Categories** - Work, Personal, Shopping, Health, Other

### Advanced Features
- 📅 **Due Dates** - Set deadlines and track overdue tasks
- 📊 **Statistics** - View progress and completion metrics
- 🌙 **Dark/Light Theme** - Toggle between themes
- ⌨️ **Keyboard Shortcuts** - Speed up your workflow
- 💾 **Local Storage** - Persistent data storage
- 📤 **Export/Import** - Backup and restore todos
- 🎨 **Responsive Design** - Works on all devices

## 🚀 Quick Start

### Prerequisites
- Node.js 16+
- npm or yarn

### Installation

```bash
# Clone repository
git clone https://github.com/fatonkamal025-dot/didactic-lamp.git
cd didactic-lamp/todo-app

# Install dependencies
npm install

# Start development server
npm run dev
```

Visit `http://localhost:5173` in your browser.

## 📁 Project Structure

```
todo-app/
├── src/
│   ├── components/
│   │   ├── TodoForm.jsx         # Add new todos
│   │   ├── TodoList.jsx         # Display todos
│   │   ├── TodoItem.jsx         # Individual todo item
│   │   ├── FilterBar.jsx        # Filter options
│   │   ├── SearchBar.jsx        # Search functionality
│   │   ├── ThemeToggle.jsx      # Dark/Light mode
│   │   ├── Stats.jsx            # Statistics dashboard
│   │   ├── Export.jsx           # Export/Import
│   │   └── KeyboardShortcuts.jsx # Shortcuts info
│   │
│   ├── hooks/
│   │   ├── useTodos.js          # Todo management
│   │   └── useKeyboard.js       # Keyboard events
│   │
│   ├── utils/
│   │   ├── storage.js           # LocalStorage utilities
│   │   └── filters.js           # Filter utilities
│   │
│   ├── App.jsx                  # Main app component
│   ├── App.css                  # App styles
│   ├── index.css                # Global styles
│   └── main.jsx                 # Entry point
│
├── index.html                   # HTML template
├── vite.config.js              # Vite config
├── tailwind.config.js          # Tailwind config
└── package.json
```

## ⌨️ Keyboard Shortcuts

| Keys | Action |
|------|--------|
| `Ctrl/Cmd + N` | Create new todo |
| `Ctrl/Cmd + F` | Focus search |
| `Ctrl/Cmd + L` | Toggle theme |
| `Enter` | Save edited todo |
| `Escape` | Cancel editing |

## 💾 Local Storage

All todos are automatically saved to your browser's local storage:
- No server required
- No account needed
- Your data stays on your device
- Persists across browser sessions

## 🎨 Tech Stack

- **React 18** - UI library
- **Vite** - Build tool
- **Tailwind CSS** - Styling
- **React Icons** - Icon library
- **LocalStorage API** - Data persistence

## 📊 Statistics

Track your productivity with:
- **Total Todos** - All tasks created
- **Active Todos** - Incomplete tasks
- **Completed Todos** - Finished tasks
- **Progress %** - Completion percentage with progress bar

## 🌙 Dark Mode

- Toggle between dark and light themes
- Preference saved to localStorage
- Auto-detects system preference on first visit
- Smooth transitions

## 📤 Export & Import

### Export
- Save all todos as JSON file
- Filename includes current date
- Perfect for backup

### Import
- Load todos from JSON file
- Overwrites existing todos
- Validates file format

## 🔍 Search & Filter

### Filters
- **All** - Show every todo
- **Active** - Show incomplete todos
- **Completed** - Show finished todos

### Search
- Real-time search as you type
- Searches by todo text
- Case-insensitive matching
- Clear button included

## 🎯 Priority Levels

Organize by importance:
- **High** - Urgent, do first
- **Medium** - Regular priority
- **Low** - Can wait

## 📁 Categories

Organize by type:
- 💼 Work
- 👤 Personal
- 🛒 Shopping
- 🏥 Health
- 📌 Other

## 📅 Due Dates

- Set deadlines for tasks
- Visual indicators for overdue tasks
- Days until due calculation
- Sort and track by due date

## 📱 Responsive Design

- Mobile optimized
- Tablet friendly
- Desktop perfect
- Touch-friendly interface

## 🚀 Build for Production

```bash
npm run build
```

Output will be in `dist/` directory.

## 📚 Documentation

- See [README.md](../README.md) for main project info
- Check [CONTRIBUTING.md](../CONTRIBUTING.md) for contribution guidelines

## 💡 Usage Tips

1. **Quick Add** - Press Ctrl/Cmd+N for fast input
2. **Search** - Use Ctrl/Cmd+F to quickly find todos
3. **Edit** - Click the edit icon on any todo
4. **Drag** - Reorganize by priority or importance
5. **Export** - Backup regularly to a JSON file
6. **Theme** - Choose dark mode for less eye strain

## 🐛 Issues & Support

- [Report a bug](https://github.com/fatonkamal025-dot/didactic-lamp/issues)
- [Request a feature](https://github.com/fatonkamal025-dot/didactic-lamp/discussions)

## 📄 License

MIT License - Free to use and modify

## 👨‍💻 Contributing

Contributions welcome! See [CONTRIBUTING.md](../CONTRIBUTING.md)

---

**Ready to boost your productivity?** 🚀 Start using Todo App now!
