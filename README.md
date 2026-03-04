# Stack Tasks

A minimalist, stack-based task manager for focused productivity. Work on one thing at a time—when something urgent comes up, push it to the top. When done, pop it off and return to what you were doing.

## Philosophy

Just like a call stack in programming, this app treats your tasks as a LIFO (Last In, First Out) structure. The task on top is your current focus. Complete it or push something more urgent above it.

## Features

- **Stack-based workflow** — Push new tasks on top, pop completed ones off
- **Time tracking** — Tracks active time only while a task is on top
- **Reorder tasks** — Move tasks up or down to reprioritize
- **Archive** — Completed tasks are archived with their time data
- **Dark mode** — Toggle between light and dark themes
- **Color palettes** — Choose from 5 accent colors (Blue, Purple, Rose, Emerald, Amber)
- **Persistent storage** — All data saved locally in your browser
- **Keyboard shortcuts** — Fast workflow with keyboard support

## Usage

### Basic Operations

| Action | How |
|--------|-----|
| Add task | Type in input field and press `Enter` or click "Push" |
| Complete top task | Click ✓ button on the top task |
| Move task up | Hover and click ↑ arrow |
| Move task down | Hover and click ↓ arrow |
| Remove task | Hover and click ✕ on non-top tasks |

### Keyboard Shortcuts

| Shortcut | Action |
|----------|--------|
| `Enter` | Push new task (when input focused) |
| `⌘/Ctrl + Enter` | Pop (complete) top task |
| `Escape` | Close modals/panels |

### Settings

Click the gear icon (⚙) in the bottom-right corner to:
- Toggle dark/light mode
- Select accent color palette

### Archive

Click "Archive" in the bottom-left to view completed tasks with:
- Completion date
- Total time spent on the task

## Tech Stack

- Vanilla HTML/CSS/JavaScript
- No dependencies
- LocalStorage for persistence
- Google Fonts (Inter)

## Running Locally

Simply open `index.html` in a browser, or serve with any static file server:

```bash
# Python
python3 -m http.server 8080

# Node.js
npx serve

# Then open http://localhost:8080
```

## Data Storage

All data is stored in browser localStorage:

| Key | Description |
|-----|-------------|
| `stack-tasks` | Current task stack |
| `stack-archive` | Completed tasks |
| `stack-theme` | Theme preference (light/dark) |
| `stack-palette` | Color palette preference |

## License

MIT
