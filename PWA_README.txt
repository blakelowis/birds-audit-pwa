# Birds Audit Tools — PWA Pack

Files created:
- `manifest.webmanifest` — Web App Manifest
- `service-worker.js` — Service worker (cache-first)
- `icons/icon-192.png`, `icons/icon-512.png` — App icons
- `pwa_RUN_THIS.html`, `pwa_AuditorApp.html`, `pwa_Scorecard.html` — originals with PWA hooks injected

## How to use
1. Upload **all** these files to the **same folder** as your existing HTMLs (e.g., SharePoint library folder).
2. Use the `pwa_RUN_THIS.html` as your entry point. Install from your browser's menu (Add to Home screen / Install app).
3. Must be served over **HTTPS** and the service worker scope must cover the HTML files (same folder).
4. If you need a different start page, change `start_url` in `manifest.webmanifest`.
5. To update the cache, bump the `CACHE_NAME` in `service-worker.js`.
