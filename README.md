# Acropolis Companion — v2.2

A GitHub Pages-ready, dependency-free, offline-first PWA for exploring the Acropolis Museum with floor-by-floor guidance, practical camera scan notes, Greek learning, and a storage-safe personal museum diary.

**Version visible in app:** `v2.2`

## What this app does

Acropolis Companion is a personal museum companion. It does **not** replace the official Acropolis Museum Digital Guide. It helps you move through the museum, understand what floor/gallery you are in, capture object photos where allowed, confirm the museum label, use guided-looking prompts, learn Greek words, and save your visit as a personal memory book.

## v2.2 upgrade

v2.2 focuses on diary safety and honest object-explainer framing.

### 1. Storage-safe diary photos

Earlier versions stored diary photos as large base64 strings inside the same `localStorage` object as the diary text. After a few photos, browser storage could fill up and saving could fail.

v2.2 changes this:

- Diary text remains in `localStorage`.
- Diary photos are stored separately in `IndexedDB`.
- The diary state now keeps only a lightweight photo reference.
- The diary loads photos asynchronously when rendering entries.
- The app wraps `save()` in `try/catch` and shows a clear warning if saving fails.

### 2. One-time photo migration

On first load, v2.2 checks for older diary entries that still contain base64 photo data inside `localStorage`.

If old photos are found, the app:

1. Copies each old photo into `IndexedDB`.
2. Replaces the old base64 photo in `localStorage` with a lightweight photo reference.
3. Keeps the diary entry text intact.

If the migration cannot move a photo for any reason, the app leaves the original photo data in place instead of deleting it. This is designed to avoid losing existing diary entries or photos.

### 3. Photo-preserving export

v2.2 keeps the existing plain-text diary export and adds a stronger backup option:

- **Export text** — exports diary text as `.txt`.
- **Export HTML + photos** — exports one self-contained `.html` file with diary text and photos embedded inline.

Use **Export HTML + photos** after your visit if you want a permanent backup that still shows your images even if browser data is later cleared.

### 4. Honest guided-looking copy

The former “Object Explainer” wording has been adjusted. The app now frames this feature as a **Guided Object Looking Tool**.

This is more accurate because the app does not contain a full museum object database. For most objects, it helps you:

- observe more carefully,
- use the museum label,
- ask better questions,
- understand object type and context,
- save your own interpretation.

The app still reminds you to confirm exact object identity with the museum label or the official Acropolis Museum Digital Guide.

### 5. Version consistency

The app uses one visible version string everywhere: `v2.2`.

## Floor-by-floor Museum Mode

The app includes a floor-by-floor structure:

- **Level -1 — Excavation Museum**
- **Ground Floor — Gallery of the Acropolis Slopes**
- **First Floor — Early History of the Acropolis**
- **First Floor — Archaic Acropolis Gallery**
- **First Floor — Periklean Monuments**
- **First Floor — Caryatids / Erechtheion**
- **First Floor — Later Acropolis**
- **Second Floor — Rest / Restaurant / Bookshop**
- **Third Floor — Parthenon Gallery**

Each floor/gallery guide includes:

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

## Practical Camera Scan

The Scan tab is a practical capture-and-confirm tool, not automatic AI object recognition.

Recommended flow:

1. Take or upload a photo.
2. Preview the photo.
3. Tap **Retake photo** if it is blurry, wrong, or not useful.
4. Confirm the museum label or official guide name.
5. Add object type, museum area, and visible clues.
6. Create a practical scan guide.
7. Send details into Guided Object Looking.
8. Save the photo and notes to the Museum Diary.

## Existing features preserved

- Practical Camera Scan
- Retake Photo button
- Floor-by-Floor Museum Mode
- Guided Object Looking Tool
- Essential Route with progress tracking
- Mark route stops done
- Save route stops to diary
- Greek Learning Mode with themed vocabulary, phrases, listening, and mini quiz
- Museum Diary with photos, editing, search, delete, text export, and HTML + photos export
- Offline-first saving
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

## Testing the v2.2 migration

Before replacing your live app, test on a copy:

1. Open your current version.
2. Add two diary entries with photos.
3. Upload v2.2 to a test GitHub Pages repo or branch.
4. Open v2.2 in the same browser profile.
5. Confirm the old diary entries still appear.
6. Confirm the old photos still appear.
7. Try **Export HTML + photos** and open the exported file.

The migration is designed not to delete old photo data unless the new IndexedDB copy succeeds and the localStorage state saves successfully.

## Important accuracy note

v2.2 is **not true AI object recognition**. The camera/photo feature helps you capture the object and move confirmed information into Guided Object Looking and the diary. For object identity, confirm with the museum label or the official Acropolis Museum Digital Guide.

## Suggested next upgrade

**v2.3 Deeper Parthenon Gallery Mode**

Possible next improvements:

- Separate Parthenon modes: Frieze, Metopes, Pediments, Missing/Surviving Pieces
- Better “original vs cast” prompts
- Stronger Parthenon-specific Greek vocabulary
- Optional “view toward the Acropolis” reflection flow
