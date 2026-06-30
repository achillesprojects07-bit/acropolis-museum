# Acropolis Companion — V1.1

**Acropolis Companion** is a lightweight, phone-friendly museum companion app for visiting the Acropolis Museum.

V1.1 adds **Museum Walk Mode**, so you can choose where you are standing inside the museum and receive a simple guide for that area.

## Version

Current version: **V1.1 — Museum Walk Mode**

The version is visible inside the app at the top-right of the header.

## Important Note

This app does **not** replace the official Acropolis Museum Digital Guide.

For object identification, use the official Acropolis Museum / Smartify guide first. This companion app is meant to help you understand what you are seeing, remember it, learn Greek from it, and save your reflections.

## Files Included

- `index.html` — the full app
- `manifest.webmanifest` — PWA install settings
- `sw.js` — offline caching service worker
- `README.md` — this guide

## What Changed in V1.1

### Added: Museum Walk Mode

New bottom tab: **Walk**

You can choose:

- Ground Floor: Slopes of the Acropolis
- Archaic Acropolis Gallery
- Caryatids / Erechtheion
- Parthenon Gallery
- Excavation Area
- Café / Reflection Break

Each area gives you:

- What this area means
- What to look for
- Nearby highlights
- Greek words
- A reflection question
- Save this area to diary

### Updated Home Screen

The home screen now highlights **V1.1 Museum Walk Mode** and includes a direct button to the new feature.

### Updated Bottom Navigation

The bottom navigation now has five tabs:

- Home
- Walk
- Object
- Greek
- Diary

### Updated Offline Cache

The service worker cache is updated to `acropolis-companion-v1-1` so GitHub Pages/iPhone Safari can refresh the new version more reliably.

## Main Features

### 1. Museum Walk Mode

Choose where you are standing and get a mini guide for that museum area.

### 2. Explain an Object

Type the object name, label text, or what the official guide says. The app can help explain:

- What it is
- Why it matters
- What to notice
- Related Greek words

### 3. Museum Routes

Choose a route based on your available time:

- 30 minutes
- 60 minutes
- 90 minutes
- 2 hours

Each route gives you a calm path and what to notice at each stop.

### 4. Greek Learning Mode

Learn simple museum-related Greek words, including:

- άγαλμα — statue
- ναός — temple
- θεά — goddess
- μάρμαρο — marble
- προσφορά — offering

### 5. Museum Diary

Save your own notes from the visit, including:

- Object or gallery name
- What you saw
- What you felt
- Greek words learned
- Favorite detail

The diary saves locally in your browser using `localStorage`.

## How to Publish on GitHub Pages

1. Create a new GitHub repository, or open your existing Acropolis Companion repository.
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
6. Wait for GitHub Pages to create or refresh your live link.
7. Open the link in Safari on your iPhone.
8. Tap **Share → Add to Home Screen** to install it like an app.

## Important When Updating From V1.0

After uploading V1.1, open the app link and refresh once. If your iPhone still shows the old app:

1. Open the GitHub Pages link in Safari.
2. Refresh the page.
3. Close and reopen the Home Screen app.
4. If needed, remove the old Home Screen icon and add it again.

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

- V1.2 Essential Acropolis Museum Route
- V1.3 Smarter Object Explainer
- V1.4 Beautiful Museum Diary
- V1.5 Greek Learning Mode upgrade
- V2.0 Camera / AI upgrade
