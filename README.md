<h1 align="center">Ledger: A Private, Offline Weight Tracker</h1>

<p align="center">
  <i>"One file. Your data. No server, no signup, no tracking."</i>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/HTML5-Structure-E34F26?logo=html5&logoColor=white" alt="HTML5 Badge">
  <img src="https://img.shields.io/badge/CSS3-Styling-1572B6?logo=css3&logoColor=white" alt="CSS3 Badge">
  <img src="https://img.shields.io/badge/JavaScript-Vanilla-F7DF1E?logo=javascript&logoColor=black" alt="JavaScript Badge">
  <img src="https://img.shields.io/badge/Storage-localStorage-4CAF50" alt="Storage Badge">
  <img src="https://img.shields.io/badge/Backend-None-lightgrey" alt="No Backend Badge">
  <img src="https://img.shields.io/badge/Works-Offline-9C27B0" alt="Offline Badge">
</p>

---

## Overview

**Ledger** is a single-file weight tracker for people who want to log a daily number without handing it to an app, a cloud database, or an account system.

There's no backend, no sign-up, and no analytics. Every entry is written straight to your browser's `localStorage`, so the whole thing works completely offline — download it, open it, and start logging. Host it if you want a stable link, or just keep the file on your machine.

*A measurement log, not a product. Your weight history stays on your device, in your browser, under your control.*

---

## Features

- **Daily logging** — date, weight (kg), and an optional note, saved instantly.
- **Trend chart** — a hand-drawn SVG line chart with a ruler-style axis, a dashed goal line, and hover tooltips, switchable across 2-week, 1-month, 3-month, and all-time ranges.
- **Calendar view** — a month grid showing which days you logged, click any day to add or edit that entry.
- **Goal tracking** — set a target weight and see how far above or below it you are at a glance.
- **Stats panel** — streak count, 7-day average, total change, highs/lows, and distance to goal.
- **Full log table** — every entry, editable and deletable, in one scrollable list.
- **Fully offline & private** — no accounts, no network calls, no analytics. Data lives only in your browser's local storage.

---

## Tech Stack

| Technology | Purpose |
|-----------------------------|------------------------------------------------|
| HTML5 | Single-page structure, no build step |
| CSS3 | All styling, self-contained, no frameworks |
| Vanilla JavaScript | Chart rendering, calendar, stats, form logic |
| Browser `localStorage` | Persistent, private, on-device data storage |
| Google Fonts (CDN) | Fraunces, Inter, IBM Plex Mono — the only external request the page makes |

---

## Core Functionality

### Logging an entry
- You enter a date, weight, and optional note in the quick-add form (or click a calendar day).
- The entry is written to `localStorage` under a single JSON key — no server round-trip.

### Rendering the trend
- On load, JavaScript reads all entries, filters them to the selected range, and computes min/max/step for the ruler axis.
- An SVG path, gradient-filled area, and goal line are built and injected directly into the DOM.

### Stats & streaks
- Streak, weekly average, and goal distance are recalculated live from the entry list every time you add, edit, or delete a record.

---

## Getting Started

### Option 1 — Just open it (fully offline)
1. **Download** `index.html` from this repo.
2. **Double-click it** — it opens in your default browser and works immediately, no internet required after the first load (fonts won't load offline, but the app itself works fine).

### Option 2 — Clone the repo
```bash
git clone https://github.com/D-Majumder/Weight_Ledger.git
cd Weight_Ledger
open index.html   # or just double-click it in your file explorer
```

### Option 3 — Host it for a stable link
Ledger is a static file, so any static host works: GitHub Pages, Netlify, Cloudflare Pages, or a folder on your own server.
```bash
# Example: GitHub Pages
# 1. Push this repo to GitHub
# 2. Settings → Pages → Deploy from branch → main / root
# 3. Visit https://d-majumder.github.io/Weight_Ledger/
```
> Note: data is stored per-browser. If you host it and use it from multiple devices, each browser keeps its own separate history.

---

## Customization Tips

- **Change the unit**: search for `kg` across `index.html` and swap in `lb` if you prefer pounds (no unit-conversion logic is built in).
- **Change the default goal**: edit the `placeholder="75.0"` value on the goal input to your own starting point.
- **Restyle it**: all colors and fonts are CSS custom properties at the top of the `<style>` block (`--bg-base`, `--brass`, `--sage`, etc.) — change the palette without touching layout code.
- **Add more fields**: entries are stored as `{date, weight, note}` objects — extend the object and the form to track things like body fat % or sleep.

---

## License

This project is released under the **MIT License** — free to use, modify, and share.
See the `LICENSE` file for details.

---

## Author

<p align="center">
  <a href="mailto:dhrubamajumder@proton.me" target="_blank">
    <img src="https://img.shields.io/badge/Email-Dhruba%20Majumder-blue?logo=gmail" alt="Email Badge">
  </a>
  <a href="https://www.linkedin.com/in/iamdhrubamajumder/" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-Dhruba%20Majumder-blue?logo=linkedin" alt="LinkedIn Badge">
  </a>
  <a href="https://github.com/D-Majumder" target="_blank">
    <img src="https://img.shields.io/badge/GitHub-D--Majumder-black?logo=github" alt="GitHub Badge">
  </a>
</p>
