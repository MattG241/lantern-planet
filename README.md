# Night Shift

A tiny cel-shaded planet you run the midnight post around, in the browser — inspired by
the vibe of [Messenger](https://messenger.abeto.co/). It's a replayable, randomized
score-attack: reach each glowing beacon before the shift clock runs out, build a combo
with fast drops, and chase a new best under a sky full of stars.

- **Play:** open `index.html` (or the live GitHub Pages link).
- **Goal:** deliver as much post as you can before the clock hits zero. Every delivery
  buys back time; fast deliveries grow your combo (and your payout). Detour to light a
  paper lantern for bonus seconds, and grab gems to keep the chain alive. Each run
  reshuffles the city and rolls a random night modifier (Rush Hour, Full Moon, Blackout,
  Meteor Shower, ...). Your best score is saved, and a finished shift returns to the
  main menu so you can dive straight into the next one.
- **Controls:** WASD / arrows to walk the planet, click for free-look (pointer lock),
  Shift to sprint, Space to hop, mouse-wheel to zoom, F for full screen. On mobile:
  left side is a virtual joystick, drag the right side to look, pinch to zoom.

Built as a single self-contained HTML file with [three.js](https://threejs.org)
(loaded from a CDN) — no build step. Cel shading via `MeshToonMaterial` + `OutlineEffect`,
a WebGL2 post chain (bloom, miniature tilt-shift DOF, Sobel ink-edge grade), a
spherical-gravity walk controller, a canvas-baked starfield night sky, and a courier
delivery loop with combos, run modifiers, and a saved high score.
