# Travel Journal

A local-first, installable travel journal combining destination records, weather history and forecasts, photographs, and personal notes.

## Version 1

- Manually search for places worldwide using Open-Meteo geocoding.
- View current conditions, the previous seven days, and the next seven days.
- Record visits with dates, notes, tags, and photographs.
- Keep data in the browser using IndexedDB; export/import a JSON backup.
- Install as a Progressive Web App on supported devices.

## Run locally

Serve this folder with any static web server (for example `python -m http.server 8000`) and open `http://localhost:8000`. Weather and geocoding require an internet connection. Photos and journal records are stored locally in the browser on that device.

## Deploy

GitHub Actions builds/deploys the static site to GitHub Pages on pushes to `main`. Enable **Settings → Pages → Build and deployment → GitHub Actions** if Pages is not already enabled.

## Data and privacy

No account or backend is required for V1. Journal entries and photos stay in the browser's IndexedDB and are not uploaded to GitHub or a third party. Use Export regularly to back up your data. Clearing browser storage or changing devices without importing a backup will lose local records.

Weather data: [Open-Meteo](https://open-meteo.com/). Historical weather is model/reanalysis data and may be delayed; it is not a guaranteed on-site station observation.
