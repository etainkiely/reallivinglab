# REAL Living Lab — GitHub Pages launch package

This folder is ready to upload to the root of the `etainkiely/reallivinglab` GitHub repository.

## Upload
Upload **the contents of this folder**, not the enclosing folder itself. Keep the `images/` directory intact.

Core files:
- `index.html` — homepage
- `styles.css` — shared visual system
- `atlas.html` — Living Atlas
- `annaghdown.html` — Annaghdown Community Garden
- `base-lab.html` — Base Lab
- `physics-farm.html` — Physic(s) Farm
- `patterns.html` — Pattern Commons
- `learning.html` — REAL Learning
- `evidence.html` — Evidence / Nature Record
- `enoll.html` — ENoLL evidence journey
- `atu.html` — For ATU
- `collaborate.html` — Join REAL
- `danu.html` — legacy redirect to Annaghdown Community Garden
- `CNAME` — preserves `reallivinglab.com` on GitHub Pages
- `robots.txt`, `sitemap.xml`, `404.html` — deployment support
- `images/` — all launch images, web-optimised and referenced by relative paths

## Verified before packaging
- all internal HTML links resolve
- all image paths resolve
- legacy `danu.html` redirects correctly
- navigation and footer cross-link the principal pages
- current-page navigation state is marked with `aria-current=page`
- external links open safely in a new tab
- ENoLL chapter labels use the 2026 terminology: Strategy; Operations; Openness; Users & Reality; Value & Impact; Stability & Harmonization
- old master tagline “Science you can walk into” is not used
- master tagline is “Learning together.”
- Base Lab and Physic(s) Farm are described as private project sites, not public visitor locations

## Important
Do not delete the `CNAME` file if `reallivinglab.com` is already configured for GitHub Pages.
