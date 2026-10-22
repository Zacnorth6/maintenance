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

## Team password (optional)
`team.json` holds the sync settings encrypted with the team password
(PBKDF2-SHA256, 600,000 rounds → AES-256-GCM). Without the password it's unreadable.
Create it in the app under Settings → Team access, then upload it here.
To change the password or lock someone out: create a new GitHub token, delete the old one,
reconnect in Settings, make a new team.json and upload it over the old one.

## Updating
Upload a new `index.html` (Add file → Upload files). GitHub Pages republishes in about a minute.
If a phone still shows the old version, close and reopen the app.
