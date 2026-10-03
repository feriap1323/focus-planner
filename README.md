# Focus Planner

A single-file, zero-dependency productivity app for planning study tasks and working through them in timed focus sessions.

## Features

- **Pomodoro-style timer** — choose 15, 25, or 45-minute sessions; pause, resume, and reset at any time.
- **Task list** — add tasks with High / Medium / Low priority, check them off, and delete them individually or clear all completed tasks at once.
- **Progress bar** — visual indicator of how many tasks are done today.
- **Session counter** — tracks how many focus sessions you finish each day.
- **Dark mode toggle** — click the **Dark / Light** button in the top-right corner to switch themes. Your preference is saved in `localStorage` and will persist between visits. The app also respects your OS-level `prefers-color-scheme` setting by default.
- **Persistent state** — tasks and session count are stored in `localStorage` and reset each new day automatically.
- **Accessible** — proper ARIA labels, live regions for the timer, and visible focus rings throughout.
- **Mobile-friendly** — responsive two-column grid that collapses to a single column on small screens; honours iOS safe-area insets.

## Usage

1. Open `Focus Planner.html` directly in any modern browser — no server, no build step, no dependencies.
2. Add tasks in the **Today's progress** panel and set a priority.
3. Pick a session length, press **Start**, and work until the timer hits zero.
4. Check off tasks as you complete them.

## File structure

```
Focus Planner/
└── Focus Planner.html   # The entire app — HTML, CSS, and JS in one file
└── README.md            # This file
```

## Browser support

Works in any browser that supports CSS custom properties and `localStorage` (all modern browsers: Chrome, Firefox, Safari, Edge).

## Dark mode

The toggle button at the top-right of the page cycles between **Light** and **Dark** mode. The chosen theme is saved to `localStorage` under the key `focus-planner-theme`. If no preference has been saved, the app automatically follows the operating-system dark-mode setting (`prefers-color-scheme`).

## Local development

No build tooling is required. Open the HTML file directly:

```
# macOS / Linux
open "Focus Planner.html"

# Windows
start "Focus Planner.html"
```

Or serve it with any static file server if you prefer:

```
npx serve .
```

## License

MIT — do whatever you like with it.
