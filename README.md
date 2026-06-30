# Acropolis Companion — V1.5 Greek Learning Mode

A GitHub Pages-ready, offline-first PWA for exploring the Acropolis Museum.

**Version visible in app:** `v1.5 Greek Learning Mode`

## What this app does

Acropolis Companion is a personal museum companion. It does **not** replace the official Acropolis Museum Digital Guide. It helps you move through the museum, understand what you are seeing, learn Greek words, and save your visit as a personal memory book.

## V1.5 upgrade

V1.5 focuses on the Museum Diary.

New / upgraded features:

- Beautiful Museum Diary screen
- Add optional photo to a diary entry
- Edit saved diary entries
- Delete saved diary entries
- Search diary entries
- Save museum area per entry
- Separate fields for:
  - What I saw
  - What I felt
  - Greek words I learned
  - Favorite detail
- Export diary as a `.txt` file
- Object Explainer photo can now be saved into the diary entry
- Version badge updated inside the app
- Service worker cache updated for GitHub Pages refresh

## Existing features preserved

- Museum Walk Mode
- Essential Route
- Route progress tracker
- Mark route stops done
- Save route stops to diary
- Smarter Object Explainer
- Greek Words Mode with el-GR speech support where available
- Offline-first localStorage saving
- GitHub Pages-ready static files

## Files included

Upload all of these files to your GitHub repository:

- `index.html`
- `manifest.webmanifest`
- `sw.js`
- `README.md`

## How to deploy on GitHub Pages

1. Create or open your GitHub repository.
2. Upload all files from this ZIP.
3. Go to **Settings → Pages**.
4. Under **Build and deployment**, choose:
   - Source: **Deploy from a branch**
   - Branch: **main**
   - Folder: **/root**
5. Save.
6. Open the GitHub Pages link.
7. On iPhone Safari, tap **Share → Add to Home Screen**.

## Important accuracy note

This app is not yet a true museum object-recognition app. For object identity, confirm with the museum label or the official Acropolis Museum Digital Guide. The app is designed as a guided interpretation, Greek-learning, and diary companion.

## Storage note

Diary entries are stored locally in the browser using `localStorage`. If the browser data is cleared, diary entries may be removed. Use **Export text** after your museum visit to save a copy.

## Suggested next upgrade

**V1.5 — Greek Learning Mode upgrade**

Recommended next improvements:

- More museum vocabulary by area
- Phrase practice for asking questions in Greek
- Mini quizzes
- Saved Greek words from diary entries
- “Words I learned today” review screen


## V1.5 Greek Learning Mode

This version upgrades the Greek tab into a mini learning path for the museum.

Added in V1.5:

- Visible app version: `v1.5 Greek Learning Mode`
- Themed Greek learning sets:
  - Core museum words
  - Statues and people
  - Temple and architecture
  - Gods and offerings
  - Useful museum phrases
- Greek words with transliteration, English meaning, and sample phrase
- Listen button using browser `el-GR` speech synthesis when supported
- Mini quiz for the selected theme
- Save Greek practice to the Museum Diary
- Updated export filename for diary text

Upload all four files to GitHub Pages and replace the old version.
