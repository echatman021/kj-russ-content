# KJ Russ Content Strategy

Home-screen app for Kj Russ, built by Citystar Productions. Shows his content niches, shoot ideas with shot lists, shoot days, and the rollout plan. Russ can send notes from inside the app.

**Live app:** https://kj-russ-content.netlify.app
**Netlify project:** kj-russ-content

## How updates work

This repo is connected to Netlify. Any change pushed to `main` publishes to the live link in about a minute. Russ keeps the same home-screen icon and gets the new version the next time he opens it.

## Where Russ's notes go

Netlify, open kj-russ-content, then Forms, then **russ-notes**. Notes live in Netlify, not in this repo, so updating the app never erases them.

## Files

| File | What it does |
|---|---|
| `index.html` | The whole app: layout, content, notes, shot checklist |
| `manifest.webmanifest` | App name, icon and colors for "Add to Home Screen" |
| `sw.js` | Lets the app open with no signal. Bump the version (`kjr-v2` → `kjr-v3`) on each update so phones grab new files |
| `netlify.toml` | Netlify settings (no build step; keeps `sw.js` from being cached) |
| `icon-*.png`, `apple-touch-icon.png` | Home-screen icons |

## Editing content

All the text lives in the `<script id="state">` block in `index.html` (niches, ideas, hooks, shots, locations, times, shoot days, rollout).

## Adding Russ to his phone (iPhone)

Open the live link in Safari, tap Share, then **Add to Home Screen**.
