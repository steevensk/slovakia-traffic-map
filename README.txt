MOBILE-SAFE PRODUCTION BUILD — Slovakia + Hungary traffic map

Upload these three files to the root of the GitHub Pages repository:
  index.html
  slovakia_traffic_2022_2023.geojson
  hungary_traffic_2024.geojson

This version keeps both national datasets external to index.html. The map UI can render immediately on phones, then loads the two GeoJSON files asynchronously.

The previous shp_su_intenzity.zip is not required.

After upload, reload the GitHub Pages URL. If the phone has cached the previous version, use a private/incognito tab once or clear the site cache.
