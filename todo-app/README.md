# Todo App - Complete To-Do List Application

A modern, feature-rich to-do list application built with React and local storage.

## 🎯 Features

- ✅ Add, edit, delete todos
- ✅ Mark todos as complete/incomplete
- ✅ Filter todos (All, Active, Completed)
- ✅ Priority levels (High, Medium, Low)
- ✅ Due dates
- ✅ Categories/Tags
- ✅ Search functionality
- ✅ Local storage persistence
- ✅ Dark/Light theme
- ✅ Statistics dashboard
- ✅ Keyboard shortcuts
- ✅ Drag & drop reordering
- ✅ Export/Import todos
- ✅ Responsive design
- ✅ Smooth animations

## 🚀 Quick Start

### Prerequisites
- Node.js 16+
- npm or yarn

### Installation

```bash
git clone https://github.com/fatonkamal025-dot/didactic-lamp.git
cd didactic-lamp/todo-app
npm install
npm run dev
```

Open [http://localhost:5173](http://localhost:5173) in your browser.

## 📋 Project Structure

```
todo-app/
├── src/
│   ├── components/
│   │   ├── TodoForm.jsx         # Add new todo
│   │   ├── TodoList.jsx         # Display todos
│   │   ├── TodoItem.jsx         # Individual todo
│   │   ├── FilterBar.jsx        # Filter options
│   │   ├── SearchBar.jsx        # Search todos
│   │   ├── ThemeToggle.jsx      # Dark/Light mode
│   │   ├── Stats.jsx            # Statistics
│   │   └── Keyboard.jsx         # Keyboard shortcuts
│   │
│   ├── hooks/
│   │   ├── useTodos.js          # Todo management logic
│   │   ├── useLocalStorage.js   # LocalStorage hook
│   │   └── useKeyboard.js       # Keyboard shortcuts
│   │
│   ├── utils/
│   │   ├── storage.js           # Storage utilities
│   │   ├── filters.js           # Filter utilities
│   │   └── helpers.js           # Helper functions
│   │
│   ├── styles/
│   │   ├── index.css            # Global styles
│   │   └── animations.css       # Animations
│   │
│   ├── App.jsx                  # Main app
│   ├── main.jsx                 # Entry point
│   └── index.css                # Global CSS
│
├── package.json
├── vite.config.js
├── tailwind.config.js
└── README.md
```

## 🎨 UI/UX

- **Dark & Light Theme** - Toggle between themes
- **Responsive Design** - Works on mobile, tablet, desktop
- **Smooth Animations** - Fade in/out, slide effects
- **Intuitive Interface** - Easy to use and navigate
- **Icons & Badges** - Visual indicators for priority and status

## 💾 Local Storage

Todos are automatically saved to browser's local storage:
- Persists across browser sessions
- Automatic backup
- Export/Import functionality
- No server required

## ⌨️ Keyboard Shortcuts

- `Ctrl/Cmd + N` - New todo
- `Ctrl/Cmd + F` - Search
- `Ctrl/Cmd + L` - Toggle theme
- `Enter` - Save todo
- `Escape` - Cancel

## 📊 Statistics

Track your productivity:
- Total todos
- Completed todos
- Active todos
- Completion percentage
- High priority count

## 📱 Responsive

- Mobile optimized
- Tablet friendly
- Desktop perfect
- Touch-friendly buttons

## 🔧 Tech Stack

- React 18
- Vite
- Tailwind CSS
- React Icons
- Local Storage API

## 📦 Package Dependencies

```json
{
  "react": "^18.2.0",
  "react-dom": "^18.2.0",
  "react-icons": "^4.11.0",
  "react-beautiful-dnd": "^13.1.1"
}
```

## 🚀 Getting Started

1. **Create a todo** - Type and press Enter
2. **Edit** - Click on todo to edit
3. **Complete** - Click checkbox to mark done
4. **Filter** - Use filter buttons to view specific todos
5. **Search** - Find todos by keyword
6. **Delete** - Remove todos

## 💡 Features Explained

### Priority Levels
- 🔴 High - Urgent todos
- 🟡 Medium - Regular todos
- 🟢 Low - Less important todos

### Filters
- **All** - Show all todos
- **Active** - Show incomplete todos
- **Completed** - Show completed todos

### Categories
Organize todos by:
- Work
- Personal
- Shopping
- Health
- Other

### Due Dates
- Set deadlines
- Visual indicators
- Sort by date

## 📚 Documentation

- [Setup Guide](./docs/SETUP.md) - Detailed setup
- [User Guide](./docs/USER_GUIDE.md) - How to use
- [Developer Guide](./docs/DEVELOPER.md) - Code structure

## 🎯 Usage Examples

### Add a Todo
```javascript
const addTodo = (text, priority, category, dueDate) => {
  // Todo is automatically saved to localStorage
}
```

### Filter Todos
```javascript
const filteredTodos = todos.filter(todo => {
  if (filter === 'completed') return todo.completed;
  if (filter === 'active') return !todo.completed;
  return true;
});
```

### Search Todos
```javascript
const searchResults = todos.filter(todo =>
  todo.text.toLowerCase().includes(searchTerm.toLowerCase())
);
```

## 🌟 Features Highlight

✨ **Clean UI** - Modern and minimal design
🎯 **Focused** - Do one thing well
⚡ **Fast** - Instant local storage
💾 **Persistent** - Never lose your todos
📱 **Responsive** - Works everywhere
♿ **Accessible** - WCAG compliant

## 🔒 Privacy

- 100% local storage
- No server uploads
- No tracking
- No analytics
- Your data, your device

## 🐛 Issues & Support

Found a bug? Have a suggestion?
- [Create an issue](https://github.com/fatonkamal025-dot/didactic-lamp/issues)
- [Start a discussion](https://github.com/fatonkamal025-dot/didactic-lamp/discussions)

## 📄 License

MIT License - Free to use and modify

## 👨‍💻 Contributing

Contributions welcome! See [CONTRIBUTING.md](../CONTRIBUTING.md)

---

**Made with ❤️ for productivity**

Start your todo app now! 🚀
