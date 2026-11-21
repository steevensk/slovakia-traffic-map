Slovakia + Hungary Traffic Map - Optimized Production Build

Upload these two files to the ROOT of the GitHub repository:

1. index.html
2. slovakia_traffic_2022_2023.geojson

The old shp_su_intenzity.zip is no longer required by the web page and may be removed from the repository after the optimized version is confirmed working.

Why this is faster:
- Slovakia is pre-aggregated from directional SSC records into 2,752 two-way counting sections.
- Only fields used by the map are retained.
- Geometry is lightly simplified (5 m tolerance) for web display.
- The browser loads map-ready GeoJSON instead of downloading/unzipping/parsing SHP + DBF on every visit.
- The GeoJSON can be cached by the browser/CDN.

Source basis remains SSC CSD 2022/2023. Traffic values are unchanged by geometry simplification.

Slovak road categories are taken directly from the official SSC road-class field:
- diaľnica / rýchlostná cesta -> Motorway / expressway
- cesta I. triedy -> Class I
- cesta II. triedy -> Class II
- cesta III. triedy and the few local/purpose records -> Class III / minor
