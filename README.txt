Slovakia + Hungary traffic map - truck exposure logic v8

Upload these three files to the GitHub repository root:
- index.html
- slovakia_traffic_2022_2023.geojson
- hungary_traffic_2024.geojson

Truck exposure adjustment:
- <250 trucks/day: no band increase
- 250-999 trucks/day: +1 band
- 1,000+ trucks/day: +2 bands
- if truck share is 30% or more and the road already has at least 250 trucks/day: +1 additional band
- total adjustment capped at +3 bands

This release keeps the mobile interaction/layout fixes from v7 unchanged.
