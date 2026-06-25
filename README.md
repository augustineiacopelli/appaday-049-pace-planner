# 049 — Pace Planner

**AppADay · Day 049 · Category: Data Viz (D)**

A personalized race training plan generator for distances from 5K to 50K. Enter your goal time, fitness level, and preferred training style, and get a complete week-by-week plan with pace targets, a mileage ramp chart, and daily workout breakdowns.

---

## What It Does

Select a race distance, set your goal finish time, describe your current fitness base, and choose a training philosophy. Pace Planner generates a full training block — 8 weeks for a 5K up to 20 weeks for a 50K — with every day planned out and every pace calculated from your goal time.

A start date picker anchors the plan to real calendar dates. Set it to your first Monday and every week header and day row shows its actual date. The start date persists between sessions via localStorage.

---

## Training Distances & Plan Lengths

| Distance | Miles | Plan Length | Peak Mileage |
|---|---|---|---|
| 5K | 3.1 mi | 8 weeks | ~25 mi/week |
| 10K | 6.2 mi | 10 weeks | ~30 mi/week |
| Half Marathon | 13.1 mi | 12 weeks | ~40 mi/week |
| Full Marathon | 26.2 mi | 16 weeks | ~50 mi/week |
| 50K Ultra | 31.1 mi | 20 weeks | ~55 mi/week |

---

## Training Styles

**Balanced** — Rooted in Hal Higdon's approach. Easy runs build aerobic base, one weekly tempo sharpens lactate threshold, and a progressive long run builds race-specific endurance.

**Polarized (80/20)** — Based on Matt Fitzgerald's research. Roughly 80% of runs at conversational easy pace, 20% at threshold or faster. Polarized training produces strong adaptation for most athletes.

**Run-Walk (Galloway)** — Jeff Galloway's strategic walk-break method. Reduces injury risk and recovery time on long runs. Particularly effective for first-time distance runners.

**Conservative** — Maximum 10% weekly mileage increases, extra rest days, no speedwork until week 4. Best for runners returning from injury or training with limited weekly hours.

---

## Pace Targets

All paces derive from your goal finish time and are adjusted for fitness level:

- **Goal Pace** — your average mile pace to hit your finish time
- **Easy Pace** — 75–105 seconds per mile slower than goal (varies by style)
- **Tempo Pace** — 10–15 seconds per mile faster than goal
- **Long Run Pace** — 60–100 seconds per mile slower than goal
- **Interval Pace** — ~20 seconds per mile faster than goal (mile race pace)

---

## Features

- Five race distances with appropriate plan lengths and mileage peaks
- Four training methodologies with real methodological foundations
- Pace key showing all five training zones calculated from goal time
- Animated weekly mileage ramp chart (area chart with taper visible)
- Week-by-week accordion with full daily workout descriptions
- Recovery weeks every 4th week built into the mileage progression
- Taper and Race Week badges with appropriate reduced volume
- Plan Start Date picker — anchors every week and day to real calendar dates
- Start date persists in localStorage between sessions
- Monday-start validation with next-Monday suggestion
- Fitness level adjustments to pace spread (advanced runners get tighter zones)
- Fully responsive — two-panel desktop, single-column mobile

---

## Tech

Single-file vanilla HTML/CSS/JS. No frameworks, no external libraries. Canvas API for the mileage chart. localStorage for start date persistence.

---

[← Back to Portfolio](https://augustineiacopelli.github.io/appaday/)
