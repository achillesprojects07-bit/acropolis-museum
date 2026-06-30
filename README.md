# Acropolis Companion — V2.1 Floor-by-Floor Museum Mode

A GitHub Pages-ready, offline-first PWA for exploring the Acropolis Museum with clearer floor guidance, practical camera scan notes, Greek learning, and a personal museum diary.

**Version visible in app:** `v2.1 Floor-by-Floor Museum Mode`

## What this app does

Acropolis Companion is a personal museum companion. It does **not** replace the official Acropolis Museum Digital Guide. It helps you move through the museum, understand what floor/gallery you are in, capture object photos where allowed, confirm the museum label, learn Greek words, and save your visit as a personal memory book.

## V2.1 upgrade

V2.1 fixes the main weakness in the earlier Museum Walk Mode: it now tells you **which floor or museum area you are talking about**.

Instead of general area names only, V2.1 adds a floor-by-floor structure:

- **Level -1 — Excavation Museum**
- **Ground Floor — Gallery of the Acropolis Slopes**
- **First Floor — Early History of the Acropolis**
- **First Floor — Archaic Acropolis Gallery**
- **First Floor — Periklean Monuments**
- **First Floor — Caryatids / Erechtheion**
- **First Floor — Later Acropolis**
- **Second Floor — Rest / Restaurant / Bookshop**
- **Third Floor — Parthenon Gallery**

Each floor/gallery guide now includes:

- Floor / level
- Gallery name
- “Where you are” explanation
- Camera rule for that area
- What the area means
- What to look for
- Nearby highlights
- Greek words
- Reflection question
- What to do next
- Save this area to diary

## Important camera rule

The app includes a special warning for the **First Floor — Archaic Acropolis Gallery**:

> Camera off here. Use text notes only.

In all other areas, the app reminds the user to follow posted museum signs, avoid flash, avoid blocking visitors, and confirm museum rules.

## Route improvements in V2.1

The Essential Route now follows the museum more clearly by floor:

1. Ground Floor — Gallery of the Acropolis Slopes
2. First Floor — Early History of the Acropolis
3. First Floor — Archaic Acropolis Gallery
4. First Floor — Periklean Monuments
5. First Floor — Caryatids / Erechtheion
6. First Floor — Later Acropolis
7. Third Floor — Parthenon Gallery
8. Second Floor — Rest / Restaurant / Bookshop
9. Level -1 — Excavation Museum

The 30-, 60-, 90-, and 120-minute route options were also updated to use these clearer floor/gallery names.

## Scan improvements preserved

V2.1 preserves the V2.0.1 **Retake Photo** fix:

1. Take or upload a photo.
2. Preview the photo.
3. Tap **Retake photo** if it is blurry, wrong, or not useful.
4. Confirm the museum label or official guide name.
5. Add object type, museum area, and visible clues.
6. Create a practical scan guide.
7. Send details into the Object Explainer.
8. Save the photo and notes to the Museum Diary.

This is still the safe practical scan version, not automatic AI object recognition.

## Existing features preserved

- Practical Camera Scan
- Retake Photo button
- Smarter Object Explainer
- Essential Route with progress tracking
- Mark route stops done
- Save route stops to diary
- Greek Learning Mode with themed vocabulary, phrases, listening, and mini quiz
- Beautiful Museum Diary with photos, editing, search, delete, and export
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

V2.1 is **not yet true AI object recognition**. The camera/photo feature helps you capture the object and move confirmed information into the explainer and diary. For object identity, confirm with the museum label or the official Acropolis Museum Digital Guide.

## Storage note

Diary entries are stored locally in the browser using `localStorage`. If the browser data is cleared, diary entries may be removed. Use **Export text** after your museum visit to save a copy.

## Suggested next upgrade

**V2.2 Deeper Parthenon Gallery Mode**

Possible next improvements:

- Separate Parthenon modes: Frieze, Metopes, Pediments, Missing/Surviving Pieces
- Better “original vs cast” prompts
- Stronger Parthenon-specific Greek vocabulary
- Optional “view toward the Acropolis” reflection flow
