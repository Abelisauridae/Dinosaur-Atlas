# Dinosaur Atlas

Static dinosaur atlas app built from PBDB occurrence data plus supplemental size enrichment.

Each species record includes a generated description summary, and exact World Dinosaur Dataset matches can also contribute a short supplemental note.
Each species also includes image metadata that points to a local family-aware silhouette.

## Open the app

Open `index.html` in a browser. The data is loaded from local JavaScript files, so it does not require a local dev server just to view it.

## Rebuild the database

1. Refresh the raw source cache in `data/raw` if you want newer source exports.
2. Run:

```bash
python3 dinosaur-atlas/scripts/build_dinosaur_data.py
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
- image coverage for all 1,855 species through local family-aware silhouettes

## Sources

- PBDB taxonomic names API for accepted species and taxonomy
- PBDB fossil occurrences API for coordinates and interval data
- World Dinosaur Dataset for length, weight, and dinosaur type enrichment
- Natural Earth 1:110m land polygons for the map backdrop
