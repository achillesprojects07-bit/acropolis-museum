# Acropolis Companion — V2.0 Practical Camera Scan

A GitHub Pages-ready, offline-first PWA for exploring the Acropolis Museum.

**Version visible in app:** `v2.0 Practical Camera Scan`

## What this app does

Acropolis Companion is a personal museum companion. It does **not** replace the official Acropolis Museum Digital Guide. It helps you move through the museum, capture object photos, confirm the museum label, understand what you are seeing, learn Greek words, and save your visit as a personal memory book.

## V2.0 upgrade

V2.0 adds **Practical Camera Scan**.

This is not automatic AI recognition yet. It is the safe museum version:

1. Take or upload a photo of the object or label.
2. Confirm the label or official guide name.
3. Add object type, museum area, and visible clues.
4. Create a practical scan guide.
5. Send the details into the Object Explainer.
6. Save the photo and notes to the Museum Diary.

## New / upgraded features in V2.0

- New **Scan** tab in the bottom navigation
- Camera/photo input with rear-camera hint on mobile
- Photo preview before saving
- Confirmed museum label field
- Object type selector
- Museum area selector
- Visible clues field
- **Create scan guide** button
- **Use in Object Explainer** button
- **Save scan to diary** button
- Scan photo can move into the Object Explainer
- Diary export filename updated to V2.0
- Visible app version updated to `v2.0 Practical Camera Scan`
- Service worker cache updated for GitHub Pages refresh

## Existing features preserved

- Museum Walk Mode
- Essential Route
- Route progress tracker
- Mark route stops done
- Save route stops to diary
- Smarter Object Explainer
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

V2.0 is **not yet true AI object recognition**. The camera/photo feature helps you capture the object and move information into the explainer and diary. For object identity, confirm with the museum label or the official Acropolis Museum Digital Guide.

## Storage note

Diary entries are stored locally in the browser using `localStorage`. If the browser data is cleared, diary entries may be removed. Use **Export text** after your museum visit to save a copy.

## Suggested next upgrade

**V2.1 AI Vision Scan**

Possible next improvements:

- Optional AI Vision API connection
- Image-based object description
- Label reading/OCR assistance
- Confidence warning for uncertain matches
- Stronger “confirm before saving” workflow
