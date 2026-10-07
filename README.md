# San Francisco billboard map

**[Open the live billboard map](https://fonduh.github.io/MappingSF/)**

The previous Overture Maps demo is preserved at [overture-3d.html](https://fonduh.github.io/MappingSF/overture-3d.html).

An interactive map of photographed billboard lettering, using the latest manually cleaned text cutouts.

Open `index.html`, or serve this directory as a static site. Everything needed to display the map is embedded in that file.

- Map scale stays at 300%; drag or scroll to move through the bounded SF–SFO area.
- Text appears when its source location is inside the viewport, with offsets and connector lines to avoid overlaps.
- Hover or tap a sign to see its full photograph, company, and source date.

The centered Silkscreen header alternates the SF letters between blue and red every two seconds (static with reduced motion). The full-width blue About bar has asymmetric square-block edges and opens the author’s essay and credits on desktop and mobile.

## Sources

The photographs and source coordinates come from [The Valley of AI](https://thevalleyofai.com/), captured October 2, 2026. Per-sign source links and any supplied photographer credits are in `sources.json`. Coordinates are archive claims, not independently verified positions; moving advertisements use source sightings.

The displayed inventory contains 38 signs with usable coordinates under the project's existing SF–SFO scope. The local archive contains 63 ads; 12 have no usable source coordinates and 10 are outside the existing scope. Three bus ads were removed from the displayed inventory at the author’s request. The remaining signs include the saved text-cutout edits.

Road geometry derives from DataSF street centerlines and the Caltrans state highway network. Faint registry markers represent the SF Planning GASP sign inventory, rather than verified current advertisements.

The map uses Leaflet, Silkscreen, and Inter; their licenses are included in `THIRD_PARTY_LICENSES.txt`. Photographs, ad creative, and third-party data retain their respective ownership and attribution. No blanket license is granted to those assets by this repository.

The retouch editor runs locally and is not part of this static publication. To publish later edits, rebuild the local map and run `staging/paper-texture/build_preview.py`, then publish its generated `index.html` with the production page title.
