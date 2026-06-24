# FLUX — Generative Particle Engine

An interactive, full-screen particle visualizer built with **React** and the HTML5 **Canvas** API. Five physically-distinct field modes, live controls, color palettes, cursor interaction, and one-click PNG export.

![modes](https://img.shields.io/badge/modes-5-22d3ee) ![react](https://img.shields.io/badge/react-18-a78bfa)

## Modes
- **Nebula** — slow, swirling flow field with long glowing trails.
- **Flow** — a finer, faster flow field — sharp, energetic streaks.
- **Vortex** — particles spiral around a central singularity.
- **Constellation** — drifting nodes that link into a living network.
- **Starfield** — warp-speed flight through space.

## Controls
- **Density / Speed / Trails** sliders.
- **Cursor force**: attract, repel, or off — move your mouse (or finger) to disturb the field.
- **Palette** cycle: Plasma, Aurora, Inferno, Ice, Solar.
- **Save PNG** of the current frame.

### Keyboard
| Key | Action |
|-----|--------|
| `Space` | play / pause |
| `R` | randomize everything |
| `S` | save a PNG |
| `M` | cycle cursor force |
| `P` | hide / show the panel |

## Run it locally
```bash
npm install
npm run dev
```
Then open the URL Vite prints (usually http://localhost:5173).

To build a static, deployable version:
```bash
npm run build      # outputs to /dist
npm run preview    # preview the production build
```
The contents of `/dist` can be dropped onto any static host (Vercel, Netlify, GitHub Pages, etc.).

## Stack
- React 18 + Vite
- lucide-react (icons)
- Zero canvas/animation dependencies — the entire fluid/flow simulation is hand-written in `src/App.jsx`.

## Tuning
Open `src/App.jsx` and look near the top for `PALETTES`, `COUNT_RANGE`, and `DEFAULTS` to change colors, particle limits, and the starting configuration.
