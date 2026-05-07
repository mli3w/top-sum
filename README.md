# ✈️ TOP SUM · Math Flight Over Marina Bay

> A free arcade-style math flight game for kids.
> Learn by flying through the correct answer.

🌐 **Play instantly in your browser:**
👉 https://mli3w.github.io/top-sum/

No install · No signup · Desktop + Mobile

---

![Top Sum Gameplay](top-sum-demo.gif)

<p align="center">
  <img src="top-sum-demo%20(0).gif" width="48%" alt="Top Sum — gameplay clip 1">
  &nbsp;
  <img src="top-sum-demo%20(1).gif" width="48%" alt="Top Sum — gameplay clip 2">
</p>

---

## 🎮 What is Top Sum?

Top Sum is a fast-paced 3D math game where learning happens through:

- movement
- focus
- timing
- flow

Instead of worksheets or flashcards, players pilot a plane through Marina Bay and steer toward the correct answer gates.

Chain correct answers together to:
- build streaks
- increase speed
- swap up to a faster plane
- trigger cinematic slow-motion moments
- unlock new flight experiences

It's less:
> "solve this question"

and more:
> **stay focused, stay in flow, don't break the streak**

---

## 🚀 30-Second Start

1. Open the link above (or `index.html` locally)
2. Pick a difficulty — **Tiny** for first-time learners, **Hard** for everyone else
3. Steer toward the gate showing the correct answer
4. Don't break the streak

---

## 🧠 Why I Built This

This started as a small project for my sister-in-law's son over a long weekend.

At the same time, I was exploring how AI can help prototype interactive ideas faster — especially small custom learning experiences for kids.

I also made a simplified Tiny Mode for my 4-year-old.

The result became:
> a free, open-source experiment in making maths feel more like play than repetition.

---

## ⚡ Features

### ✈️ Arcade Flight Gameplay
- Fly through the correct answer gates
- Wrong answers or collisions cost lives
- Fast restart loop designed for "one more run"

### 🔥 Flow System
- Consecutive correct answers increase your multiplier (×1 → ×2 → ×3 → ×4)
- Dynamic speed scaling
- "Flow State" visual effects and slow-motion moments

### 🛩 Plane Upgrades on Streaks
Five plane tiers swap in automatically as your streak builds:

| Streak | Plane Tier |
|-------:|:-----------|
| 0      | Tier 1 (starter) |
| 3      | Tier 2 |
| 5      | Tier 3 |
| 10     | Tier 4 |
| 20     | Tier 5 (top of the line) |

Lose your streak and you drop back. Stay in flow to keep flying the best plane.

### 🌆 Cinematic Marina Bay World
- Stylised Singapore skyline (Merlion, bay, boats, water)
- Day and Sunset modes
- Fireworks during sunset
- A Chinook with a Singapore flag orbits at altitude during the day
- Occasional NDP-style RSAF fighter formation flypast with contrails
- Dynamic lighting and atmosphere

### 🎮 Built for Desktop + Mobile
- Keyboard controls (arrows / WASD)
- Mobile joystick
- Mobile D-pad alternative
- First-time onboarding for younger kids
- Pause / resume from anywhere

### 🚀 Progression & Unlocks
- High-score persistence (localStorage, no signup)
- **Sunset Mode** unlocks at 1000 points with a cinematic celebration
- Streak milestones with visual rewards
- Score sharing (Web Share API, with clipboard fallback)

---

## 🧮 Math Levels

| Level      | Range / Operations                       | Best for              |
|------------|------------------------------------------|-----------------------|
| **Tiny**   | 1+1 → 5+5                                | 4–5 yrs, first-timers |
| **Easy**   | Addition up to ~20                       | Lower primary         |
| **Medium** | Addition + Subtraction up to ~50         | Mid primary           |
| **Hard**   | Addition, Subtraction, Multiplication    | Upper primary and up  |

---

## 🎯 Controls

### Desktop
| Key | Action |
|-----|--------|
| `← ↑ → ↓` or `WASD` | Steer |
| `M` | Toggle sound |
| `C` | Toggle auto-center |
| `T` | Toggle Day / Sunset |
| `Esc` | Pause / resume |

### Mobile
- **Joystick** (default) or **D-pad** — switch from the title screen, or via the icon column in-game
- Tap ⏸ to pause

---

## 🧩 Tech Stack

- Pure HTML / CSS / JavaScript
- WebGL via [Three.js](https://threejs.org)
- Fully client-side — no backend, no analytics, no tracking
- Single-file architecture (`index.html`)

Requires a modern browser with WebGL — Chrome, Safari, Firefox, or Edge on desktop or recent mobile.

---

## 🚀 Run Locally

No build step, no dependencies. Just clone and open:

```bash
git clone https://github.com/mli3w/top-sum.git
cd top-sum

# macOS
open index.html

# Windows
start index.html

# Linux
xdg-open index.html
```

That's it.

---

## ⚖️ Disclaimer

Top Sum is an independent fan-style aviation tribute. It is **not affiliated with, endorsed by, or sponsored by Paramount Pictures or the Top Gun franchise** — the visual style draws on the broader military-aviation design language only.

---

## 📜 License

[MIT](LICENSE) — fork it, remix it, build on it. If you make something fun for your own kids with it, that would make my day.

---

## ❤️ Made with love for my kids
