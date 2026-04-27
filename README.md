# 🏃 Marathon Training Log

A fully interactive, browser-based 20-week marathon training tracker with integrated strength training — built as a single HTML file with zero dependencies beyond an internet connection for fonts.

> **No server. No login. No app store.** Just open the link and train.

---

## Live Demo

**[Launch Training Log →](https://JobinJohn24.github.io/marathon-training-log/marathon_training_log.html)**

---

## What This Is

A personal training dashboard designed for someone running their first (or next) marathon while maintaining a strength training routine. It tracks every workout across all 20 weeks, remembers exactly where you left off, and celebrates milestones along the way.

The plan is structured around four phases:

| Phase | Weeks | Focus |
|-------|-------|-------|
| Base Building | 1–4 | Aerobic foundation, introduce lifting |
| Build | 5–10 | Increase mileage and training volume |
| Peak | 11–16 | Highest mileage weeks, race-specific work |
| Taper | 17–20 | Reduce load, stay sharp for race day |

---

## Weekly Workout Structure

Each week follows this split:

| Day | Type | Description |
|-----|------|-------------|
| Monday | Strength | Lower Body — squats, deadlifts, lunges |
| Tuesday | Run | Easy Run — 60–70% max HR |
| Wednesday | Strength | Upper Body — bench, rows, shoulder press |
| Thursday | Run | Tempo Run or Intervals |
| Friday | Strength / Cross | Conditioning or Cross-Training (taper weeks) |
| Saturday | Run | Long Run — the most important workout of the week |
| Sunday | Rest | Full rest, stretch, foam roll |

Recovery weeks fall on Weeks 4, 8, 12, and 16 — mileage drops roughly 25% to let your body absorb the training load.

---

## Equipment Used

All workouts are designed around this specific setup:

| Equipment | Used For |
|-----------|----------|
| Power Rack + Barbell (225 lb) | Back Squat, Bench Press, Bent-Over Row, RDL |
| Hex Bar | Hex Bar Deadlift, Farmer Carries |
| PowerBlock Dumbbells | Lunges, Shoulder Press, Curls, Core Work |
| Treadmill | Easy runs, Tempo runs, Long runs (weather backup) |
| Rowing Machine | Conditioning circuits, warm-up rows |
| Stationary Bike | Active recovery, low-impact cross-training |
| Jump Rope | Conditioning circuits, warm-up, footwork |

---

## Features

### Workout Logging
- Click any day card to open the full exercise list
- Check off individual exercises as you complete them
- Log actual miles and time for every run
- Write session notes in a free-text field
- Mark the full day complete when done

### History and Session Tracking
- Every action is timestamped and saved to the History tab
- Tracks when you first started the log
- "Last Action" strip in the sidebar shows what you did and when
- Session opens are recorded automatically

### Celebration System
- **Exercise check** — particle burst fires from the checkbox
- **Day complete toast** — randomized motivational message slides in from the bottom-right
- **Week complete modal** — full-screen celebration with confetti, phase color, and weekly stats
- **Milestone achievements** — unlock pop-up cards at 25%, 50%, and 75% plan completion
- **Phase completion banners** — drop from the top when you finish a phase block
- **Streak badge** — pulsing fire icon tracks consecutive completed weeks
- **Week crown** — completed weeks in the sidebar get a crown icon

### Progress Tracking
- Weekly mileage target bar chart, color-coded by phase
- Phase breakdown doughnut chart
- Live overall plan completion percentage in the top bar

### Data Persistence
- All progress saves to your browser's `localStorage` automatically
- No account, no server, no sync required
- Every return to the same URL in the same browser restores your full progress

---

## Mileage Plan

Weekly target mileage across all 20 weeks:

```
Wk 1:  15 mi   Wk 6:  25 mi   Wk 11: 35 mi   Wk 16: 30 mi
Wk 2:  18 mi   Wk 7:  28 mi   Wk 12: 25 mi   Wk 17: 32 mi
Wk 3:  20 mi   Wk 8:  20 mi   Wk 13: 38 mi   Wk 18: 25 mi
Wk 4:  15 mi   Wk 9:  30 mi   Wk 14: 40 mi   Wk 19: 18 mi
Wk 5:  22 mi   Wk 10: 33 mi   Wk 15: 42 mi   Wk 20: 10 mi
```

Peak mileage is at Week 15 (42 miles). The taper begins at Week 17.

---

## Data Storage Notes

Because this app uses `localStorage`:

- Progress persists every time you return to the **same URL** in the **same browser**
- Works completely offline once the page has loaded
- Clearing browser site data will erase your log
- Switching browsers starts a fresh log
- Incognito / private windows do not save anything
- Another person visiting your GitHub Pages link gets their own clean, separate log

**Recommendation:** Bookmark the GitHub Pages URL and always open it from the same browser.

---

## File Structure

```
marathon-training-log/
├── marathon_training_log.html   ← The entire app
└── README.md                    ← This file
```

The entire application lives in a single HTML file. No build process, no npm, no configuration needed.

---

## Tech Stack

| Layer | Choice |
|-------|--------|
| UI | Vanilla HTML, CSS, JavaScript |
| Charts | Chart.js 4.4.1 via CDN |
| Fonts | Barlow Condensed, Barlow, Source Code Pro via Google Fonts |
| Storage | Browser localStorage |
| Hosting | GitHub Pages |
| Dependencies | None |

---

*Built with Claude · Trained with grit*
