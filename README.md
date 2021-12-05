# Accesible routes (hopefully)

The geojson source uses the following overpass turbo query exported as geojson:
```
way[highway=path][surface][surface!=dirt][surface!=grass][surface!=unpaved][surface!=mud][surface!=ground](area:3606195356);
out geom;
```
