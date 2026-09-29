<h1 align="center">Ledger: A Private, Offline Weight & Gym Workout Tracker</h1>

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

**Ledger** is a single-file weight and gym workout ledger for people who want to track their fitness, bodyweight, weekly workout timetable, and daily attendance without handing data over to cloud servers, subscription apps, or account systems.

There's no backend, no sign-up, and no analytics. Every entry is written straight to your browser's `localStorage`, so the whole thing works completely offline — download it, open it, and start logging. Host it if you want a stable link, or just keep the file on your machine.

*A personal measurement & training log, not a product. Your fitness history stays on your device, in your browser, under your control.*

---

## Features

### 🏋️ Gym Timetable & Workout Attendance Tracker
- **Customizable Weekly Split Timetable** — define your muscle group schedule for Monday through Sunday (e.g. Chest & Triceps, Back & Biceps, Legs, Shoulders, Full Body, Rest).
- **1-Click Split Presets** — choose from popular training templates including Push/Pull/Legs (PPL), 5-Day Bro Split, Upper/Lower, Full Body 3x, and Arnold Split.
- **Daily Attendance Logging** — mark workouts as **Completed ✓**, **Absent / Skipped ✕** (with skip reason), or **Rest Day ☕**.
- **Attendance & Consistency Analytics** — track how many days you worked out vs. skipped, your consistency percentage score, active workout streaks, and total gym hours.
- **Muscle Group Distribution** — visual breakdown of training frequency across muscle groups (Chest, Back, Legs, Shoulders, Arms, Core, Cardio).
- **Interactive Workout Calendar** — monthly grid with color-coded badges for completed sessions, absent days, and rest days.
- **Full Workout History Log** — filterable history log with edit and delete support.

### ⚖️ Weight Tracker
- **Daily logging** — date, weight (kg), and an optional note, saved instantly.
- **Trend chart** — a hand-drawn SVG line chart with a ruler-style axis, a dashed goal line, and hover tooltips, switchable across 2-week, 1-month, 3-month, and all-time ranges.
- **Calendar view** — a month grid showing which days you logged, click any day to add or edit that entry.
- **Goal tracking** — set a target weight and see how far above or below it you are at a glance.
- **Stats panel** — streak count, 7-day average, total change, highs/lows, and distance to goal.
- **Full log table** — every entry, editable and deletable, in one scrollable list.

### 📊 Unified Overview & Backup
- Combined metrics showing both weight trends and gym attendance side-by-side.
- **Export & Import (JSON)** — backup your data anytime with one click.
- **Demo Data Generator** — load sample workout history and weight logs to explore all analytics instantly.
- **Fully offline & private** — no accounts, no network calls, no analytics. Data lives only in your browser's local storage.

---

## Tech Stack

| Technology | Purpose |
|-----------------------------|------------------------------------------------|
| HTML5 | Single-page structure, no build step |
| CSS3 | All styling, self-contained, responsive luxury dark theme |
| Vanilla JavaScript | Chart rendering, timetable management, attendance analytics, calendar logic |
| Browser `localStorage` | Persistent, private, on-device data storage |
| Google Fonts (CDN) | Fraunces, Inter, IBM Plex Mono — the only external request the page makes |

---

## Getting Started

### Option 1 — Just open it (fully offline)
1. **Download** `index.html` from this repo.
2. **Double-click it** — it opens in your default browser and works immediately, no internet required after the first load.

### Option 2 — Clone the repo
```bash
git clone https://github.com/D-Majumder/weight-ledger.git
cd weight-ledger
open index.html   # or double-click index.html in file explorer
```

### Option 3 — Host on GitHub Pages
```bash
# Push this repo to GitHub
# Settings → Pages → Deploy from branch → main / root
```

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
