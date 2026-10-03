# San Francisco billboard map

**[Open the live billboard map](https://fonduh.github.io/MappingSF/)**

The previous Overture Maps demo is preserved at [overture-3d.html](https://fonduh.github.io/MappingSF/overture-3d.html).

An interactive map of photographed billboard lettering, using the latest manually cleaned text cutouts.

Open `index.html`, or serve this directory as a static site. Everything needed to display the map is embedded in that file.

- Map scale stays at 300%; drag or scroll to move through the bounded SF–SFO area.
- Text appears when its source location is inside the viewport, with offsets and connector lines to avoid overlaps.
- Hover or tap a sign to see its full photograph, company, and source date.

## Sources

The photographs and source coordinates come from [The Valley of AI](https://thevalleyofai.com/), captured October 2, 2026. Per-sign source links and any supplied photographer credits are in `sources.json`. Coordinates are archive claims, not independently verified positions; moving advertisements use source sightings.

The displayed inventory contains 41 signs with usable coordinates under the project's existing SF–SFO scope. The local archive contains 63 ads; 12 have no usable source coordinates and 10 are outside the existing scope. This published map incorporates seven manually retouched signs from the latest set of 13 saved archive edits.

Road geometry derives from DataSF street centerlines and the Caltrans state highway network. Faint registry markers represent the SF Planning GASP sign inventory, rather than verified current advertisements.

The map uses Leaflet; its license is included in `THIRD_PARTY_LICENSES.txt`. Photographs, ad creative, and third-party data retain their respective ownership and attribution. No blanket license is granted to those assets by this repository.

The retouch editor runs locally and is not part of this static publication. To publish later edits, rebuild the local map and replace `index.html` with the generated `sf-billboards-map.html`.
