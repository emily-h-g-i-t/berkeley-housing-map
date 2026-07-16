# Cal Housing Map

An interactive map and dashboard for exploring UC Berkeley's on-campus student housing — residence halls, undergraduate apartments, graduate apartments, and family housing.

**[View the live site →](https://amily307.github.io/berkeley-housing-map/)**

## What it does

- Plots all 19 UC Berkeley campus housing complexes on a map, color-coded by who's eligible to live there (undergraduate, graduate, or family housing)
- Lets you filter by eligibility, housing type (residence hall vs. apartment), and meal plan inclusion
- Lets you sort by price, distance to campus, or name
- Click a pin or a card in the sidebar to see full details: room types, price range, amenities, dining, theme programs, and eligibility requirements

## Data covered

| Category | Buildings |
|---|---|
| Undergraduate residence halls | Unit 1, Unit 2, Unit 3, Foothill, Stern, Clark Kerr, Blackwell Hall, Martinez Commons |
| Undergraduate apartments | Channing-Bowditch, Enclave, Panoramic Berkeley, New Sequoia, Wada, Helen Diller Anchor House (transfer-only) |
| Graduate apartments | Ida L. Jackson, Intersection, Manville, xučyun ruwway (grad-priority, limited undergrad) |
| Family student housing | University Village (Albany) |

Rates reflect UC Berkeley Housing's projected 2026–27 academic year rates, sourced from [housing.berkeley.edu](https://housing.berkeley.edu). Room types, amenities, and eligibility rules are compiled from official UC Berkeley Housing pages.

## Tech

Single self-contained `index.html` file — no build step, no dependencies to install.

- [Leaflet.js](https://leafletjs.com/) + OpenStreetMap tiles for the map
- Vanilla HTML/CSS/JS for filtering, sorting, and the detail panel
- All housing data is embedded directly in the file as JSON

## Running it locally

Just open `index.html` in any browser — no server required.

## Notes & limitations

- Coordinates are approximate (derived from street addresses, not precisely geocoded). Good enough for a campus-scale map, but not survey-accurate.
- Prices are projected rates and subject to change — always confirm current rates at [housing.berkeley.edu/rates-contracts-policies/rates](https://housing.berkeley.edu/rates-contracts-policies/rates/).
- A few complexes (e.g. Intersection Apartments) didn't have a precise street address published, so their pin location is a best estimate.
- This is an independent, unofficial project — not affiliated with or endorsed by UC Berkeley Housing.

## Contributing

Found outdated info or a wrong coordinate? Open an issue or a PR with a source link and it'll get fixed.
