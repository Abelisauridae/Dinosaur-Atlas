# Dinosaur Atlas

GitHub-ready package for the Dinosaur Atlas prototype.

This folder contains the static site, generated data, image fallbacks, and the rebuild script used to regenerate the dataset.

## What is included

- `index.html` - app entry point
- `app.js` - client-side app logic
- `styles.css` - layout and visual design
- `data/` - generated dinosaur database plus land geometry
- `images/fallbacks/` - family-aware dinosaur silhouette fallbacks
- `scripts/build_dinosaur_data.py` - dataset rebuild script
- `data/raw/` - cached source exports used by the generator

## Open the app locally

Open `index.html` in a browser.

## Rebuild the database

Run:

```bash
python3 scripts/build_dinosaur_data.py
```

The generator writes:

- `data/dinosaur-database.json`
- `data/dinosaur-database.js`
- `data/world-land.json`
- `data/world-land.js`

## Current dataset coverage

- 1,855 accepted species from the PBDB `Dinosauria^Aves` feed
- 1,733 species with mapped fossil coordinates
- 4,733 aggregated fossil localities
- 296 exact size matches
- 140 genus-proxy size matches
- image coverage for all 1,855 species through matched artwork or family-aware local fallbacks

## Publish help

- GitHub repo and GitHub Pages steps: `GITHUB_SETUP.md`
- Apple App Store planning notes: `APPLE_APP_STORE_PLAN.md`
