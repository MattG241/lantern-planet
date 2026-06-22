# Lantern Planet

A tiny cel-shaded planet you can walk around in the browser, inspired by the vibe of
[Messenger](https://messenger.abeto.co/). Stroll a courier around a little round world
and light all the lanterns.

- **Play:** open `index.html` (or the live GitHub Pages link).
- **Controls:** WASD / arrows to walk the planet, drag to look, mouse-wheel to zoom,
  Shift to stroll, Space to hop. On mobile: left side of the screen is a virtual
  joystick, drag the right side to look.

Built as a single self-contained HTML file with [three.js](https://threejs.org)
(loaded from a CDN) — no build step. Cel shading via `MeshToonMaterial` + `OutlineEffect`,
spherical-gravity walk controller, a flat teal void with paper-grain overlay, and a
gentle "light the lanterns" goal with a wisp companion.
