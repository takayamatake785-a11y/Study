# Study Quest v3.0

Installable, offline-capable study tracker and lightweight RPG.

## v3 additions
- Monster bestiary with discovery and defeat records
- Six evolutionary families and rank metadata (lower to calamity)
- Upper-rank encounters are uncommon in normal exploration and more frequent in dungeons
- Rarity tiers (normal / rare / legendary) are independent of monster rank
- Six original fantasy monster illustrations embedded in index.html, so no asset folder upload is needed
- Bestiary filters and branching evolution-tree views

## Deploy to GitHub Pages from iPhone
Upload the six files in this folder to the root of the existing `study-quest` repository, replacing same-named files: `index.html`, `manifest.webmanifest`, `sw.js`, `icon-192.png`, `icon-512.png`, and `README.md`. No subfolders are required.

## Data
Progress is stored in browser localStorage. Export a JSON backup from Settings before clearing site data or changing devices. Existing v2 data uses the same storage key and is migrated with empty bestiary records.
