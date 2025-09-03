# The Silver Stone Castle Quest — GitHub Pages Bundle

This folder is ready to upload directly to a GitHub repository and host with **GitHub Pages**.

## Quick Deploy (Web UI)
1) Go to https://github.com/new and create a repo, e.g. `silverstone-quest` (Public is fine).
2) Click **"Add file" → "Upload files"** and drag-drop **ALL files from this folder** (keep them at the repo root).
3) Commit the upload.
4) Go to **Settings → Pages**:
   - **Source**: "Deploy from a branch"
   - **Branch**: `main` (or `master`), **Folder**: `/ (root)`
   - Save.
5) After it builds, your site will be live at:  
   `https://<your-username>.github.io/silverstone-quest/`

## Open on iPhone (Chrome)
- Open the URL above in Chrome on your iPhone.
- Use the Share menu to bookmark it. (If "Add to Home Screen" isn't visible in Chrome, it's an iOS limitation — bookmarking still works.)
- The app runs fully client-side.

## Files
- `index.html` — app shell (pulls data from embedded JSON at load)
- `styles.css` — theme
- `app.js` — logic & localStorage
- `castle_codes.json` — generated codes for all levels
- `castle_codes.csv`, `levels.csv` — data exports
- `logo.png` — your logo
- `.nojekyll` — disables Jekyll processing on Pages
- `README.txt` — usage notes

## Staff Passcode (Demo)
- Default: `1234` (change the value in `index.html` near `window.QUEST_CONFIG`).

## Notes
- Everything is static and works without a backend.
- For production, swap the staff passcode with a secure server-side check and real payment at the kiosk.
