# Budget Tracker

A mobile-friendly monthly budget tracker — a single-page PWA with no build step and no dependencies.

**Features**

- Checklist budget: tick items as payments are made; items with subtasks (e.g. Fees → school, Qari Sahib, Sipara) complete automatically when every subtask is checked
- Record the **actual amount paid** when it differs from the budget; over/under is tracked per item and in the totals
- Extra-expense logging against any category, with a running "extra spent" total
- Report view: budget vs paid vs difference per item, extras breakdown and out-of-pocket total — for the current month and any saved month
- Month archiving: starting a new month saves the finished month exactly as it was — checkmarks, extras and totals — browsable any time in a view-only history
- Edit any item or subtask (name, amount, note) and reorder items with move up / down
- Light / dark blue theme with a one-tap toggle (follows system preference by default)
- Installable on the home screen (web app manifest + icons) and works offline after first load (service worker)

- Backup and restore via a JSON file — also the way to move data between devices

**Privacy:** all data is stored in the browser's localStorage on the user's own device. Nothing is sent anywhere.

**Hosting:** plain static files — deploy the repo root on Vercel, Netlify or GitHub Pages with zero configuration.

| File | Purpose |
|---|---|
| `index.html` | The entire app (markup, styles, logic) |
| `sw.js` | Service worker — offline caching |
| `manifest.json`, `icon-*.png` | Install metadata and app icons |
