# Rally 833 (app version)

Your HTML game packaged as an installable web app (PWA).

## How to play / install

1. Open the game in any browser (e.g. via GitHub Pages, if enabled).
2. On a phone (Android/Chrome or iOS/Safari): use the browser menu → **Add to Home Screen**. It installs like a normal app, runs fullscreen, and works offline.
3. On a computer (Chrome/Edge): click the **install** icon in the address bar.

## What was changed from the original HTML

- three.js (r128) is now served locally (`three.min.js`) instead of from a CDN.
- The Google Fonts (Saira Condensed 500/700/800, Share Tech Mono 400) are embedded in `fonts.css` as data URLs.
- Added `manifest.webmanifest` (name, colors, fullscreen launch) and app icons (`icon-*.png`, `apple-touch-icon.png`, `favicon-32.png`).
- Added `sw.js`, a service worker that caches everything, so the game works with no internet after first load.

The game itself (all scripts, 3D models and logic in `index.html`) is untouched.
