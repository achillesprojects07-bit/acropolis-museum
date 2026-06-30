# Acropolis Companion

**Acropolis Companion** is a lightweight, phone-friendly museum companion app for visiting the Acropolis Museum.

It is designed to help you explore the museum with more meaning, not just identify objects. You can type an exhibit name or label, choose a route, learn useful Greek vocabulary, and save your own museum diary notes.

## Important Note

This app does **not** replace the official Acropolis Museum Digital Guide.

For object identification, use the official Acropolis Museum / Smartify guide first. This companion app is meant to help you understand what you are seeing, remember it, learn Greek from it, and save your reflections.

## Files Included

- `index.html` — the full app
- `manifest.webmanifest` — PWA install settings
- `sw.js` — offline caching service worker
- `README.md` — this guide

## How to Publish on GitHub Pages

1. Create a new GitHub repository.
2. Upload these files to the root of the repository:
   - `index.html`
   - `manifest.webmanifest`
   - `sw.js`
   - `README.md`
3. Go to **Settings → Pages**.
4. Under **Build and deployment**, choose:
   - **Source:** Deploy from a branch
   - **Branch:** main
   - **Folder:** /root
5. Click **Save**.
6. Wait for GitHub Pages to create your live link.
7. Open the link in Safari on your iPhone.
8. Tap **Share → Add to Home Screen** to install it like an app.

## Main Features

### 1. Explain an Object
Type the object name, label text, or what the official guide says. The app can help explain:

- What it is
- Why it matters
- What to notice
- Related Greek words

### 2. Museum Routes
Choose a route based on your available time:

- 30 minutes
- 60 minutes
- 90 minutes

Each route gives you a more guided way to move through the museum.

### 3. Greek Learning Mode
Learn simple museum-related Greek words, including:

- άγαλμα — statue
- ναός — temple
- θεά — goddess
- μάρμαρο — marble
- προσφορά — offering

### 4. Museum Diary
Save your own notes from the visit, including:

- Object or gallery name
- What you saw
- What you felt
- Greek words learned
- Favorite detail

The diary saves locally in your browser using `localStorage`.

## Offline Use

The app includes a service worker file, `sw.js`, so it can work offline after it has been opened once in the browser.

For best results:

1. Open the app while you still have internet.
2. Wait for the page to fully load.
3. Add it to your iPhone Home Screen.
4. Use it during the museum visit.

## Photography Reminder

Always follow the Acropolis Museum’s photography rules. Some museum areas may restrict photography, and flash/tripods/professional equipment may not be allowed.

## Future Upgrade Ideas

Possible next versions:

- Add real AI image analysis
- Add OCR for reading museum labels
- Add voice narration
- Add Greek audio pronunciation
- Add a built-in map-style museum route
- Add favorite objects
- Export diary notes as PDF

## Version

Initial GitHub-ready version: **v1.0**
