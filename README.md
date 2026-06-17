# ✦ ChappyFlow

> Your cute, professional daily planning companion — plan your day, check things off, and wrap up with intention.

![React](https://img.shields.io/badge/React-18-0D9488?style=flat-square&logo=react&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-134E4A?style=flat-square)

---

## What is ChappyFlow?

ChappyFlow is a lightweight daily planner built with React. It gives you a clean space to lay out everything you need to do in a day, track your progress as you go, and jot down any thoughts along the way. No accounts, no clutter — just you and your day.

---

## Features

- **Task management** — Add tasks with a category and priority level, check them off as you go, and delete once you no longer need
- **Progress tracking** — A live progress bar and percentage show how much of your day is done at a glance
- **Priority system** — Color-coded dots (red, amber, green) let you see what needs attention first
- **Category tags** — Organize tasks under Work, Personal, Health, or Other
- **Filter view** — Switch between All, Pending, and Done to focus on what matters right now
- **Day Notes** — A free-text section to write intentions, reflections, or anything on your mind
- **Animated check** — A satisfying bloom animation when you complete a task

---

## Tech Stack

- [React 18](https://react.dev/) with hooks (`useState`)
- [Inter](https://fonts.google.com/specimen/Inter) + [Playfair Display](https://fonts.google.com/specimen/Playfair+Display) via Google Fonts
- Plain CSS-in-JS (no external UI library)
- No backend — fully runs in the browser

---

## Getting Started

### Prerequisites

Make sure you have [Node.js](https://nodejs.org/) (v16 or higher) and npm installed.

### Installation

```bash
# Clone the repository
git clone https://github.com/your-username/chappyflow.git

# Move into the project folder
cd chappyflow

# Install dependencies
npm install
```

### Running locally

```bash
npm run dev
```

Then open [http://localhost:3000](http://localhost:3000) in your browser.

### Build for production

```bash
npm run build
```

This creates an optimized build in the `/build` folder, ready to deploy.

---

## Project Structure

```
chappyflow/
├── public/
│   └── index.html
├── src/
│   ├── ChappyFlow.jsx     # Main app component
│   └── index.js           # React entry point
├── package.json
└── README.md
```

---

## Using the App

1. **Add a task** — Click the `+ Add Task` button, type what you need to do, choose a category and priority, then press Save (or hit Enter)
2. **Check it off** — Click the circle next to any task to mark it complete; the progress bar updates instantly
3. **Filter your view** — Use the All / Pending / Done tabs to focus on different parts of your list
4. **Write a note** — Click Edit in the Day Notes section to jot down thoughts, then click Done to save
5. **Remove a task** — Hover over any task to reveal the trash icon, then click it to delete

---

## Customization

All colors, fonts, and category options are defined at the top of `ChappyFlow.jsx` — easy to adjust without digging through the code.

```js
// Change the category list
const CATEGORIES = [
  { label: "Work", color: "#0D9488", bg: "#CCFBF1" },
  { label: "Personal", color: "#0891B2", bg: "#CFFAFE" },
  { label: "Health", color: "#10B981", bg: "#D1FAE5" },
  { label: "Other", color: "#6B7280", bg: "#F3F4F6" },
];

// Change the daily quote
const QUOTE = "Small steps every day lead to big changes.";
```

---

## Roadmap

- [ ] Persist tasks with `localStorage` so they survive a page refresh
- [ ] Date picker to plan ahead or review past days
- [ ] Drag-to-reorder tasks
- [ ] Recurring tasks
- [ ] End-of-day summary modal
- [ ] Habit tracker section

---

## License

MIT — free to use, modify, and share.

---

<p align="center">Made with teal and intention</p>