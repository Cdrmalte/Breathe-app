# Breathe — iPad web app

This folder contains the first installable web-app version of Breathe.

## Included
- `index.html` — app interface, timers, phase editor, speech and chimes
- `manifest.json` — Home Screen app metadata
- `sw.js` — offline app-shell caching
- `icon.svg` — app icon

## Important
This is a prototype, not a native App Store app. It uses browser speech synthesis and localStorage. iPadOS may suspend audio/timers when the app is backgrounded, so the app pauses when it detects it has been hidden. Export exercise backups from Settings.

## Publish using an iPad
The files must be hosted over HTTPS for service-worker offline support. One option is GitHub Pages:
1. Sign in or create an account at https://github.com
2. Create a public repository named `breathe-app`.
3. Upload all four files from this folder to the repository root (extract the ZIP first in the Files app).
4. Open repository Settings → Pages.
5. Choose deploy from the `main` branch and `/ (root)`, then save.
6. After publishing, open the provided `https://...github.io/breathe-app/` URL in Safari.
7. Tap Share → Add to Home Screen. If offered, enable “Open as Web App”, then tap Add.

Publishing services and their interfaces can change. Do not include private information in a public repository.
