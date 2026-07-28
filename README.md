# Budget Tracker

A mobile-friendly monthly budget tracker — a single-page PWA with no build step and no dependencies.

**Features**

- Checklist budget: tick items as payments are made; items with subtasks (e.g. Fees → school, Qari Sahib, Sipara) complete automatically when every subtask is checked
- Extra-expense logging against any category, with a running "extra spent" total
- Month archiving: starting a new month saves the finished month exactly as it was — checkmarks, extras and totals — browsable any time in a view-only history
- Light / dark blue theme with a one-tap toggle (follows system preference by default)
- Installable on the home screen (web app manifest + icons) and works offline after first load (service worker)

**Privacy:** all data is stored in the browser's localStorage on the user's own device. Nothing is sent anywhere.

**Hosting:** plain static files — deploy the repo root on Vercel, Netlify or GitHub Pages with zero configuration.

| File | Purpose |
|---|---|
| `index.html` | The entire app (markup, styles, logic) |
| `sw.js` | Service worker — offline caching |
| `manifest.json`, `icon-*.png` | Install metadata and app icons |
