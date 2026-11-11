# MONOFLOW

A personal productivity workspace for habits, goals, focus sessions, and everyday finances.

## Run locally

1. Download this branch as a ZIP from GitHub and extract it.
2. Open the extracted folder in VS Code.
3. Start a local web server (for example, the **Live Server** extension) and open `index.html`.
4. Keep the browser tab on the local server URL while testing.

A local server is recommended because service workers and installable PWA features do not work reliably when opening the HTML file directly with `file://`.

## Your data and backups

- MONOFLOW currently stores its workspace in the browser's local storage.
- Data is local to that browser profile and device. It does **not** automatically sync between your PC, tablet, and phone.
- Use the in-app **Export JSON Backup** action regularly and keep the downloaded file somewhere safe.
- Restoring a backup replaces the current workspace after confirmation.
- Resetting the workspace and clearing the expense ledger require confirmation.

## Offline behaviour

The service worker pre-caches the app shell and can serve the main page offline after the app has been opened successfully online at least once. Fonts, Tailwind, and Chart.js are loaded from external CDNs and may not be available offline.

## Development status

This is a personal-use project under active development. Responsive layouts and the offline layer still need hands-on browser/device testing. Do not treat the app as a verified secure vault for passwords or highly sensitive information.
