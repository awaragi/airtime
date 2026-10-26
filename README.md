# Airtime

Two stopwatches, one running at a time, to compare how long each person talks. Single static page, no backend, no build.

- Tap a side to start it; tap the active side to pause.
- Space switches to the other side. Left/Right arrows pick a side directly.
- Each side has its own colour; light and dark themes follow the system.
- Long-press (3s) anywhere to reset, after a confirmation. The same dialog has "Refresh app" to clear the cache and reload an installed copy.
- State is kept in `localStorage`, so a reload keeps the times (and a running timer keeps counting).
- Keeps the screen awake whenever the app is open (Wake Lock, where supported).
- Installable PWA (manifest + service worker, works offline, portrait-locked where supported). The layout is always two wide panels stacked top and bottom and scales as you resize the window.

Install: serve over HTTPS (or localhost) and use the browser's Install / Add to Home Screen option.

Version: shown in the corner of the reset dialog. Bump it in `index.html` (`.ver`) and the `CACHE` name in `sw.js` on every change.

Run: open `index.html`, or `python3 -m http.server` and visit it from a phone on the same network.
