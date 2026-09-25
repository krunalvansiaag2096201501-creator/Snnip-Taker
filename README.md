# Snip Taker

A lightweight, local-first snippet library for Windows 10 and 11. Save text, code, URLs, and notes; organize them into collections; search and copy them whenever you need them.

## Run locally

Requires Node.js 20 or newer:

```bash
npm install
npm start
```

Use **Ctrl+Shift+S** to bring the app to the front. Data is stored locally in the app's browser storage and never sent to a server.

## Build Windows executables

On a Windows machine:

```bash
npm install
npm run dist
```

The `dist` directory contains:

- `Snip-Taker-1.0.0-x64.exe` — portable executable
- `Snip-Taker-Setup-1.0.0-x64.exe` — Windows installer

The GitHub Actions workflow at `.github/workflows/build-windows.yml` builds both targets automatically on pushes to `main` and uploads them as the `snip-taker-windows` artifact. Open the repository's **Actions** tab, select a successful workflow run, and download the artifact.

## Features

- Create, edit, delete, favorite, and copy snippets
- Tags, collections, full-text search, and recent snippets
- Optional source URL
- Offline/local-only storage
- Ctrl+N, Ctrl+K, and Ctrl+Shift+S shortcuts
