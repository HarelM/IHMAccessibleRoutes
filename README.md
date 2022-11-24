# Accesible routes (hopefully)

This uses the IHM data srouce to present accessible routes, the following overpass query might be needed, but is not in use right now.


The geojson source uses the following overpass turbo query exported as geojson:
```
(
  way[highway=path][surface][surface!=dirt][surface!=grass][surface!=unpaved][surface!=mud][surface!=ground](area:3606195356);
  way[highway=footway][surface][surface!=dirt][surface!=grass][surface!=unpaved][surface!=mud][surface!=ground](area:3606195356);
  way[highway=cycleway][surface][surface!=dirt][surface!=grass][surface!=unpaved][surface!=mud][surface!=ground](area:3606195356);
);
out geom;
```
