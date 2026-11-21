Mobile layout fix v3

Upload these three files to the GitHub repository root, replacing the existing versions:
- index.html
- slovakia_traffic_2022_2023.geojson
- hungary_traffic_2024.geojson

Fix: on screens <=768px the map wrapper now explicitly fills the viewport. The previous mobile CSS changed the app from grid to block layout, causing the relatively positioned map wrapper to collapse to zero height because the map itself was absolutely positioned.
