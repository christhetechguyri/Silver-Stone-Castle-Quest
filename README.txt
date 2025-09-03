# The Silver Stone Castle Quest — Prototype

This is a **fully offline** prototype you can open in any modern browser (iPhone, iPad, or desktop). It demonstrates:

- Blacklight purchase & user registration (name/email)
- Level-based castle code entry (only current level's codes are accepted)
- Random codes per level (5 chars, excluding 'O' and '0')
- Level completion -> Kiosk unlock flow (staff passcode required)
- Staff tools (view codes for the current level, unlock next level)
- Branding with your logo

## How to Use
1. Unzip the package.
2. Open `index.html` in a browser.
3. Tap **Get Started** → fill in **name & email** → **Activate & Begin**.
4. Enter codes for **Level 1** (see Staff screen for demo codes).
5. After finishing Level 1, go to **Kiosk** and enter staff passcode: `1234` (change in `index.html` if needed).
6. Unlock **Level 2** and continue.

## Files
- `index.html` – main app
- `styles.css` – visual theme
- `app.js` – game logic (localStorage only)
- `castle_codes.csv` & `castle_codes.json` – generated codes
- `levels.csv` – level counts, unlock costs, and prizes
- `logo.png` – your provided logo

## Notes
- This is a **client-side prototype**. For production, you’ll host the app and connect to a backend (Glide/Adalo, Airtable, Firebase, or your own API).
- Codes are stored in `castle_codes.json` and bundled into `index.html` at build time for demo.
- Kiosk payment is simulated by staff passcode entry. Replace with your actual payment/unlock workflow later.
