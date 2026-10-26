# Airtime

Two stopwatches, one running at a time, to compare how long each person talks. Single static page, no backend, no build.

- Tap a side to start it; tap the active side to pause.
- Space switches to the other side. Left/Right arrows pick a side directly.
- Long-press (3s) anywhere to reset, after a confirmation.
- Click a name to rename it. Totals and percentages update live.
- State is kept in `localStorage`, so a reload keeps the times (and a running timer keeps counting).
- Keeps the screen awake whenever the app is open (Wake Lock, where supported).
- Installable PWA (manifest + service worker, works offline). The layout is always two panels side by side and scales as you resize the window.

Install: serve over HTTPS (or localhost) and use the browser's Install / Add to Home Screen option.

Run: open `index.html`, or `python3 -m http.server` and visit it from a phone on the same network.
