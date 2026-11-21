Mobile-safe production fix v2

Upload these three files to the repository root, replacing the existing versions:
- index.html
- slovakia_traffic_2022_2023.geojson
- hungary_traffic_2024.geojson

Changes:
- mobile stats sheet is fully hidden until a road is tapped
- Leaflet JavaScript uses fallback hosts instead of failing on one CDN
- critical Leaflet layout CSS is embedded in index.html
- a visible error message is shown if all map-library hosts are blocked

After uploading, test once in a private/incognito tab to bypass cached index.html.
