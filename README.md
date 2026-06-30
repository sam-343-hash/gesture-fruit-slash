# 🍉 Fruit Slash – Hand Gesture Fruit Cutting Game

A browser-based fruit cutting game controlled entirely by your **hand gestures** via webcam. No mouse needed — just swipe your index finger through the air to slice fruits!

![Fruit Slash Banner](https://img.shields.io/badge/Hand%20Gesture-Controlled-00e5ff?style=for-the-badge)
![MediaPipe](https://img.shields.io/badge/MediaPipe-Hands-ff9500?style=for-the-badge)
![No Install](https://img.shields.io/badge/No%20Install-Open%20in%20Browser-2ecc40?style=for-the-badge)

---

## 🎮 How to Play

1. Open `index.html` in any modern browser (Chrome recommended)
2. Click **Start Game** — allow webcam access when prompted
3. Hold your hand in front of the camera
4. **Swipe your index finger** fast across fruits to slice them
5. Avoid 💣 bombs — hitting one costs a life!
6. Score combos by slicing multiple fruits in quick succession

### Controls
| Action | Input |
|--------|-------|
| Slice fruit | Move index finger fast through fruit |
| Navigate menu | Mouse or touch (fallback) |

---

## ✨ Features

- **Real-time hand tracking** via [MediaPipe Hands](https://mediapipe.dev) (runs entirely in-browser)
- **Glowing blade trail** follows your index fingertip
- **8 fruit types** with juice particle effects on slice
- **Bomb avoidance** — dodge the 💣!
- **Combo system** — 3+ fruits = 2× points + fire indicator 🔥
- **Progressive difficulty** — spawn rate increases as your score rises
- **Mouse/touch fallback** — works without a camera for testing
- **Mirrored camera feed** overlay (low opacity) so you can see your hand position
- Single-file — no build step, no server required

---

## 🚀 Getting Started

### Play Instantly (GitHub Pages)
If deployed via GitHub Pages, just open:
```
https://<your-username>.github.io/<repo-name>/
```

### Run Locally
```bash
git clone https://github.com/<your-username>/fruit-slash.git
cd fruit-slash

# Option A: Python simple server (recommended)
python3 -m http.server 8080
# Open http://localhost:8080

# Option B: Node.js
npx serve .
# Open the URL shown

# Option C: Just open index.html directly
open index.html   # macOS
start index.html  # Windows
```

> **Note:** WebRTC (camera) requires either `localhost` or `https://`. Opening `index.html` as a `file://` URL may block camera access in some browsers. Use a local server for best results.

---

## 🛠️ Tech Stack

| Tech | Use |
|------|-----|
| **MediaPipe Hands** | Real-time hand landmark detection |
| **HTML5 Canvas** | Game rendering (4 layered canvases) |
| **Vanilla JavaScript** | Game logic, physics, particle system |
| **CSS3** | UI, animations, score pops |

No frameworks. No build tools. One file.

---

## 📁 Project Structure

```
fruit-slash/
├── index.html      # Everything — game, styles, logic
└── README.md       # This file
```

---

## 🌐 Deploy to GitHub Pages

1. Push this repo to GitHub
2. Go to **Settings → Pages**
3. Set source to **main branch / root**
4. Your game is live at `https://<username>.github.io/<repo>/`

---

## 🤝 Contributing

Pull requests welcome! Ideas:
- [ ] High score leaderboard (localStorage)
- [ ] Multi-hand support (two-handed slicing)
- [ ] Power-ups (freeze time, double points)
- [ ] Sound effects
- [ ] Mobile layout

---

## 📄 License

MIT — free to use, modify, and share.
