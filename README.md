# Paint & Page — A drawing Book App

A single-tier coloring book web app with 5 hand-drawn pages: **umbrella, hut, mango, lotus, and butterfly**. Tap a color from the paint tray, then tap any part of the sketch to fill it in.

## What "Single-Tier" Means

Everything — the drawings, the coloring logic, and the page state — runs entirely in the browser. No backend, no database, no build tools.

```
Browser (HTML + CSS + JS)
   └── SVG line-art illustrations
   └── Color-fill logic (click a color → click a shape)
   └── In-memory page state (which shape is which color)
``

## Features

- 5 pages, each a hand-drawn SVG sketch with multiple fillable regions
- A paint tray of 8 colors plus an eraser
- Page navigation with back/next buttons and dot indicators
- "Clear this page" to reset just the current drawing
- Fully responsive, works on mobile and desktop
- Keyboard accessible (swatches and shapes are focusable)

## How to Run

```bash
git clone https://github.com/rashmi-rve/<repo-name>.git
cd <repo-name>/coloring-book-app
```

Then open `index.html` in any browser — no installation needed.

## File Structure

```
coloring-book-app/
├── index.html         # Complete app (HTML + CSS + JS, all 5 pages)
├── README.md          # This file
└── screenshots/
    └── (add your screenshots here)
```

## Notes

- Coloring is **in memory only** — refreshing the page resets all pages. This is expected for a single-tier app with no storage backend.
- Each illustration is built as a real SVG with separate fillable `<path>` regions (not a generic shape), so colors stay neatly inside the lines.

## Tech Used

- HTML5 + SVG
- CSS3 (custom properties, no framework)
- Vanilla JavaScript (no libraries)
- Fonts: Fredoka (headings), Nunito (body) via Google Fonts

## Author

Rashmi


