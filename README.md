# Smart To-Do List

> 🧠 AI-powered task management with an innovative, intuitive interface


A beautifully designed task management application featuring AI-powered priority detection, smart filtering, and a premium dark mode interface.


---

## ✨ Features

### 🤖 Smart Features
- **AI Priority Detection** - Automatically detects task urgency from keywords
- **Automatic Tag Extraction** - Use #hashtags for instant organization
- **Smart Filtering** - Filter by status, priority, category, or search
- **Intelligent Sorting** - Sort by priority, due date, or alphabetically
- **Overdue Alerts** - Visual warnings for late tasks
- **LocalStorage Persistence** - Tasks auto-save and survive page refreshes

### 🎨 Premium UI/UX
- **Dark Mode Theme** - Sophisticated glassmorphic design
- **Smooth Animations** - 10+ micro-interactions throughout
- **Responsive Design** - Optimized for mobile, tablet, and desktop
- **Real-time Statistics** - Live progress tracking dashboard
- **Inline Editing** - Edit tasks directly in the list
- **Color-Coded System** - Visual priority indicators

---

## 🚀 Quick Start

### Prerequisites
- Node.js 14+ 
- npm or yarn



## 📖 Usage

### Creating Tasks
1. Type your task in the input field
2. Use keywords like "urgent", "important" for auto-priority detection
3. Add #hashtags for automatic organization
4. Click "More Options" to set priority, category, and due date
5. Press Enter or click "Add Task"

### Managing Tasks
- **Complete**: Click the circle checkbox
- **Edit**: Click the pencil icon for inline editing
- **Delete**: Click the trash icon
- **Filter**: Use the filter chips or search bar
- **Sort**: Choose from the sort dropdown menu

---

## 🎯 Key Features Explained

### AI Priority Detection
The app analyzes your task text:
- Words like "urgent", "asap", "critical" → **High Priority** 🔴
- Words like "maybe", "someday" → **Low Priority** 🔵
- Everything else → **Medium Priority** 🟡

**Example:**
```
Input: "Fix critical bug ASAP"
Output: High Priority task with red indicator
```

### Tag System
Add hashtags anywhere in your task:
```
Input: "Buy groceries #shopping #health"
Output: Task with 2 searchable tags
```

### Due Date Intelligence
- Shows "Today" or "Tomorrow" for nearby dates
- Red pulsing badge for overdue tasks
- Yellow badge for tasks due within 2 days

---

## 🛠️ Tech Stack

- **Frontend:** React 18.2
- **Build Tool:** Vite 4.4
- **Icons:** Lucide React
- **Styling:** Vanilla CSS with custom properties
- **Fonts:** Google Fonts (Inter, Poppins)
- **Storage:** LocalStorage API

---

## 📁 Project Structure

```
smart-todo-list/
├── src/
│   ├── components/
│   │   ├── Header.jsx          # App header with branding
│   │   ├── Stats.jsx           # Statistics dashboard
│   │   ├── TaskInput.jsx       # Task creation form
│   │   ├── FilterBar.jsx       # Search & filter controls
│   │   ├── TaskList.jsx        # Task list container
│   │   └── TaskItem.jsx        # Individual task component
│   ├── App.jsx                 # Main app component
│   ├── App.css                 # App-level styles
│   ├── index.css               # Global design system
│   └── main.jsx                # Entry point
├── public/                     # Static assets
├── index.html                  # HTML template
├── vite.config.js             # Vite configuration
└── package.json               # Dependencies
```

---

## 🎨 Customization

### Change Colors

Edit `src/index.css` and modify the CSS variables:

```css
:root {
  --accent-primary: #6366f1;  /* Your color */
  --bg-primary: #0a0e1a;      /* Your background */
}
```

### Add Categories

Edit `src/components/TaskInput.jsx`:

```jsx
<option value="custom">🎯 Custom Category</option>
```

### Modify AI Keywords

Edit `src/components/TaskInput.jsx`, find `suggestPriority()`:

```javascript
const urgentWords = ['urgent', 'asap', 'your-keyword'];
```

---

## 🚀 Deployment

### GitHub Pages

```bash
npm run build
git add dist -f
git commit -m "Deploy to GitHub Pages"
git subtree push --prefix dist origin gh-pages
```

### Vercel

```bash
npm install -g vercel
vercel --prod
```

### Netlify

```bash
npm run build
# Drag & drop the 'dist' folder to https://app.netlify.com/drop
```

See [DEPLOYMENT.md](DEPLOYMENT.md) for detailed instructions.

---

## 📊 Performance

- **Bundle Size:** ~65KB (gzipped: ~20KB)
- **Lighthouse Score:** 95+
- **Performance:** 60fps animations
- **Load Time:** < 1s on fast connections

---

## 🌐 Browser Support

- ✅ Chrome 90+
- ✅ Firefox 88+
- ✅ Safari 14+
- ✅ Edge 90+

---



---

## 🤝 Contributing

Contributions are welcome! Feel free to:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---



## 🙏 Acknowledgments

- Icons by [Lucide](https://lucide.dev/)
- Fonts from [Google Fonts](https://fonts.google.com/)
- Built with [React](https://reactjs.org/) and [Vite](https://vitejs.dev/)



<div align="center">
  <sub>Built with ❤️ using React</sub>
</div>



