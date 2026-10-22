# Maintenance Tracker

A phone-friendly tracker for room maintenance: floor map, issue log, quarterly
room inspections, all-room projects and a parts list.

This repository only holds the app. **No maintenance data is stored here.**
Data is kept in the browser and, if sync is set up, in a separate *private*
repository (one `data.json` file) using a GitHub fine-grained access token.

## Files
- `index.html` – the whole app
- `sw.js` – lets the app open when Wi-Fi drops
- `manifest.webmanifest`, `icon-*.png`, `apple-touch-icon.png` – "Add to Home Screen" icon

## Updating
Upload a new `index.html` (Add file → Upload files). GitHub Pages republishes in about a minute.
If a phone still shows the old version, close and reopen the app.
