# Book Nook - a cute Pomodoro timer

A cute, cozy Pomodoro timer for people who'd rather be reading. Built with **React** and **Electron**, Book Nook sits on your desktop as a little companion that flips through its pages while you focus, and curls up sleeping when it's time for a break.

![status](https://img.shields.io/badge/status-in%20development-orange)
![made with](https://img.shields.io/badge/made%20with-React%20%2B%20Electron-purple)

---

## ✨ Features

- **Pomodoro-style focus timer** — work in focused sprints with built-in break intervals
- 📚 **Animated book companion** — a pixel-art book that comes alive as you work
- **Native desktop app** — runs as a standalone window via Electron, not just a browser tab
- **Cozy, minimal UI** — designed to feel like a little reading nook, not a productivity dashboard

---

## 🛠️ Tech Stack

- [React](https://react.dev/) — UI and timer logic
- [Electron](https://www.electronjs.org/) — desktop app shell and native window controls
- TypeScript (typed `window.electronAPI` bridge between renderer and main process)

---

### Prerequisites

- [Node.js](https://nodejs.org/) (LTS recommended)
- npm

> ```bash
> npm uninstall electron
> npm install electron@30 --save-dev
> rm -rf node_modules package-lock.json
> npm install
> ```

### Installation

```bash
git clone <https://github.com/mompho/book-nook>
cd book-nook
npm install
```

### Running in development

Start the React dev server:
```bash
npm start
```

In a separate terminal, launch Electron:
```bash
npm run electron
```

### Building for production

```bash
npm run build
```

This creates an optimised production build of the React app in `build/`, ready to be packaged into a distributable Electron app.

---

## 🗂️ Project Structure

```
book-nook/
├── public/
│   └── electron.js       # Electron main process entry point
├── src/
│   ├── App.tsx            # Main timer UI and logic
│   ├── electron.d.ts      # TypeScript declarations for window.electronAPI
│   └── ...
├── package.json
└── README.md
```

---

Made with 🤎 for cozy, focused reading sessions. [React documentation](https://reactjs.org/).
