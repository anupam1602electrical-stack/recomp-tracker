# Recomp Tracker — PWA Package

This package is prepared from the current Recomp Tracker V2 Android project's HTML asset.

## What changed
- Converted the V2 HTML into a Progressive Web App (PWA).
- Replaced the Android-only `window.storage` dependency with browser/device `localStorage` so workout and metric data can persist in a normal PWA.
- Added `manifest.json` for installable Android web-app packaging.
- Added an offline service worker.
- Added 192px and 512px app icons.
- Added mobile/PWA metadata.

## How to use
1. Upload this folder to an HTTPS web host. GitHub Pages, Netlify, Vercel, Cloudflare Pages, or another static HTTPS host can work.
2. Open the hosted URL on Android Chrome.
3. Confirm the app loads and that a test entry survives a refresh.
4. For an Android package, open the hosted URL with PWABuilder and use its Android packaging flow.

## Important
The PWA must be served over HTTPS (or localhost during local testing). Opening `index.html` directly as a `file://` URL will not activate the service worker.
