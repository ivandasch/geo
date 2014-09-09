ogr2ogr -f GeoJSON map.json PG:'host=host user=user dbname=dbname password=password' "table_name";
topojson --no-stitch-poles -o map.topo.json -p -s 1e-7 -- name=map.json;



