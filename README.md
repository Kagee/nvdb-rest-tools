Different tools for working with https://www.vegvesen.no/nvdb/api/

# Tools
* xml
 * Uses GET to query for data, specifies XML as return type
* json
 * Uses GET to query for data, specifies JSON as return type
* linestring-to-geojson
 * Looks for a LINESTRING in vegObjekt/lokasjon/geometriWgs84 and outputs this as GeoJSON

# Examples
* ./xml 'vegobjekter/objekt/119380248' | ./linestring-to-geojson > 119380248.json
 * Create a GeoJSON file containg the LINESTRING of object 119380248 (RV 4, south of Gjøvik)
