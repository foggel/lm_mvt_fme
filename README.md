# lm_mvt_fme
Access Lantmäteriets vector tile service from FME

This repository contains some FME examples to consume and convert the vector tile services at Lantmäteriet.
The tile service is an WMTS service offering a well known tilematrix for EPSG:3857. The service requires basic austentication.


# download_mvttileset.fmw
https://github.com/foggel/lm_mvt_fme/blob/main/download_mvttileset.fmw: 

This workspace downloads a rectangular extent from to WMTS-service and writes the tiles to a local tileset

  **Parameters:**
  XMIN: Minimum X-coordinate for the extent to download

  YMIN: Minimum Y-coordinate for the extent to download

  XMAX: Maximum ..

  YMAX: Maximum ..

  TILEMATRIX: Zoomlevel, integer betten 14 and 17

  AUTH_USERNAME: Username for http basic authentication

  AUTH_PASSWORD: Password for http basic authentication

# mtv_tileset_to_geojson.fmw
https://github.com/foggel/lm_mvt_fme/blob/main/mvt_tileset_to_geojson.fmw: 

This workspace read a local tileset and convert it to GeoJson. One GeoJson file will be written for each layer in the MVT-tileset.
