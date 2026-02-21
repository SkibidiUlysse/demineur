<p align="center">
  <h1 align="center">💣 Demineur</h1>
  <p align="center"><strong>The classic minesweeper, built from scratch with Pygame.</strong></p>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Pygame-00C853?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Genre-Puzzle-9C27B0?style=for-the-badge" />
</p>

<p align="center"><em>Left click to reveal. Right click to flag. Don't blow up.</em></p>

---

## How It Works

```
┌───────────────────────────────────────┐
│           GAME LOOP                   │
│                                       │
│   Init 8×8 grid                       │
│   Place mines randomly                │
│   Compute neighbor counts             │
│         │                             │
│         ▼                             │
│   ┌─────────────┐                     │
│   │  Wait for   │◀──────────────┐     │
│   │  player     │               │     │
│   │  input      │               │     │
│   └──────┬──────┘               │     │
│          │                      │     │
│     ┌────┴────┐                 │     │
│     ▼         ▼                 │     │
│  Left      Right                │     │
│  Click     Click                │     │
│     │         │                 │     │
│     ▼         ▼                 │     │
│  Reveal    Toggle               │     │
│  cell      flag                 │     │
│     │                           │     │
│  ┌──┴──┐                        │     │
│  ▼     ▼                        │     │
│ Mine? Empty?                    │     │
│  │     │                        │     │
│  ▼     ▼                        │     │
│ BOOM  Flood-fill ───────────────┘     │
│  💀   reveal                          │
│       neighbors                       │
│                                       │
│   All safe cells revealed? → 🏆 WIN  │
└───────────────────────────────────────┘
```

## Features

| Feature | Description |
|---------|-------------|
| **8×8 grid** | Classic board with randomly placed mines |
| **Recursive reveal** | Click an empty cell → auto-reveals all connected safe cells |
| **Flag system** | Right-click to mark suspected mines |
| **Neighbor count** | Numbers 1-8 show how many adjacent mines |
| **Win detection** | Game detects when all safe cells are uncovered |
| **Game over** | Mines revealed in red on explosion |

## Quick Start

```bash
git clone https://github.com/SkibidiUlysse/demineur.git
cd demineur

pip install pygame
python demineur.py
```

## Controls

| Action | Input |
|--------|-------|
| Reveal a cell | Left click |
| Place / remove flag | Right click |

## Roadmap

- [ ] **Difficulty selector** — Easy (8×8), Medium (16×16), Hard (24×24)
- [ ] **Timer & best times** — track personal records per difficulty
- [ ] **First-click safety** — guarantee first click is never a mine
- [ ] **Custom themes** — dark mode, retro, neon
- [ ] **Animations** — smooth reveal transitions, explosion particles
- [ ] **Sound effects** — click, flag, explosion audio feedback

---

<p align="center"><em>Simple. Addictive. Explosive.</em></p>
