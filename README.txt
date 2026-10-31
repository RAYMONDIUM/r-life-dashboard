R · Life Dashboard — offline PWA package

Contents:
- index.html: your original dashboard, with PWA manifest and service-worker registration added
- manifest.json: app name, icon, display and theme settings
- service-worker.js: caches the app shell for offline use
- icon-192.png and icon-512.png: app icons

Important:
1. Publish these files together at the root of an HTTPS website (for example, a GitHub Pages site).
2. Open the HTTPS address in Chrome on Android while online once.
3. Wait for the page to finish loading, then use Chrome menu > Install app (or Add to Home screen).
4. Open the installed app once while online. Then test by turning on Airplane mode and reopening it.

The dashboard stores its data in browser localStorage. Browser storage is tied to the installed site's origin and browser profile. Do not clear Chrome/site data or uninstall the app unless you have exported/backed up your dashboard data. This package does not add cloud sync or automatic backup.

The HTML references Google Fonts externally; the dashboard will use a fallback font if that font is unavailable offline.
