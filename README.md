# Airtime

Two stopwatches, one running at a time, to compare how long each person talks. Single static page, no backend, no build.

- Tap a side to switch to it; tap the active side to pause.
- Space switches to the other side. Left/Right arrows pick a side directly.
- Click a name to rename it. Totals and percentages update live.
- State is kept in `localStorage`, so a reload keeps the times (and a running timer keeps counting).
- Keeps the screen awake while running (Wake Lock, where supported).

Run: open `index.html`, or `python3 -m http.server` and visit it from a phone on the same network.
