# Goal Countdown

> A high-focus, aesthetic milestone roadmap and live T-minus countdown tracker engineered for ambitious career goals and technical interview preparation.

![Goal Countdown Status](https://img.shields.io/badge/status-active-emerald)
![License](https://img.shields.io/badge/license-MIT-blue)
![Stack](https://img.shields.io/badge/tech-HTML5%20%7C%20TailwindCSS%20%7C%20Tone.js-amber)

---

## 🌟 Overview

**Goal Countdown** is a self-contained, client-side dashboard designed to transform daunting goals into disciplined daily execution. Built with a dark atmospheric aesthetic and responsive glassmorphism, it combines a real-time T-minus countdown, a reverse-engineered milestone timeline, an integrated focus sprint timer, and structured engineering scratchpads.

---

## ✨ Features

- ⏳ **Live T-Minus Precision Countdown Clock**: Real-time countdown tracking days, hours, minutes, and seconds to your target date.
- 🗺️ **Backward Prep Roadmap**:
  - Structured milestones with planned study hours, subtasks, and category tags.
  - Support for travel blackout dates and target milestones.
  - Weighted overall readiness calculation based on completed hours and milestones.
  - Interactive custom confirmation modal for resetting milestones.
- ⏱️ **Daily Focus Sprint Timer**:
  - Focus presets: **60m Deep Focus Sprint**, **25m Rapid Drill**, and **10m Neural Recovery Break**.
  - Dynamic schedule mode: automatically switches between **Weekday** (2×60m = 2h target) and **Weekend** (4×60m = 4h target).
  - Web Audio feedback via [Tone.js](https://tonejs.github.io/) (gentle synthesized chimes upon sprint and milestone completion).
  - Auto-logs completed 60-minute sprint blocks upon timer completion.
- 📝 **Engineering Prep Scratchpad**:
  - Tabbed note-taking for **System Design**, **STAR Leadership Stories**, and **AI & RAG Architecture**.
  - Preloaded templates for rapid note capture and interview checklists.
  - Auto-saving with debounce indicator to `localStorage`.
  - One-click copy notes to clipboard.
- 💾 **100% Client-Side & Zero-Config**:
  - All state persists seamlessly in browser `localStorage`.
  - No database or backend infrastructure required.
  - Completely responsive on desktop, tablet, and mobile displays.

---

## 🚀 Quick Start

### Option 1: Open Directly in Browser
You can open `index.html` directly in any modern web browser:
```bash
# macOS
open index.html

# Linux
xdg-open index.html

# Windows
start index.html
```

### Option 2: Run with Node / npm
```bash
# Start a local static server
npm start
# or
npx serve .
```

### Option 3: Run with Python
```bash
python3 -m http.server 8080
```
Then navigate to `http://localhost:8080`.

---

## 📁 Project Structure

```text
countdown/
├── index.html                           # Primary web application entry point
├── t_minus_countdown_job_i_tracker.html # Original application tracker file
├── package.json                         # Project metadata and run scripts
├── .gitignore                           # Git ignore rules for OS and dependencies
├── LICENSE                              # MIT License
└── README.md                            # Project documentation
```

---

## ⚙️ Customization Guide

All configuration options are defined cleanly inside the `<script>` section of `index.html`:

1. **Target Date**:
   Change the `TARGET_DATE` constant:
   ```javascript
   const TARGET_DATE = new Date('2026-12-14T09:00:00');
   ```

2. **Milestones & Sprints**:
   Edit the `DEFAULT_MILESTONES` array to adjust dates, titles, subtasks, and allocated study hours.

3. **Scratchpad Templates**:
   Modify `NOTE_TEMPLATES` to fit your specific discipline, company targets, or study topics.

---

## 🛠️ Tech Stack

- **Styling**: [Tailwind CSS](https://tailwindcss.com/) (CDN) with custom dark atmospheric gradients and glassmorphism.
- **Typography**: [Inter](https://fonts.google.com/specimen/Inter) and [JetBrains Mono](https://fonts.google.com/specimen/JetBrains+Mono).
- **Icons**: [Font Awesome 6](https://fontawesome.com/).
- **Audio**: [Tone.js](https://tonejs.github.io/) synthesized Web Audio API.

---

## 📄 License

This project is open-source and licensed under the [MIT License](LICENSE).
