# day-2-geopandas

- [X] Why is geopandas required?
- [X] what is geopandas
- [X] how to install geopandas

## What is Geopandas
- Geopandas is open-sourced library and enables the use and manipulation of geospatial data in Python
-  It extends the common datatype used in pandas to allow for the many and unique geometric operations: GeoSeries and GeoDataFrame.
- Geopandas is also built on top of shapely for its geometric operation; its underlying datatype allows Geopandas to run blazingly fast and is appropriate for many machine learning pipelines that require large geospatial datasets.
> GeoPandas basically adds geospatial abilities to pandas

- The toughest part of geopandas is not using geopandas but installing the dependencies
- geopandas sits on top of various libraries
    1. pandas - deals with data analysis
    2. shapely - a library that deals with geometric shapes (built on software called GEOS)
    3. fiona - a software package for reading and writing files (any kind of geographic format except for a csv files) (built on OGR)
    4. pyproj - deals with cartographic projections (base on PROJ.4)
    5. descartes - mapping 
    6. geopy - geocoding (convert location names to lat and long)
    7. rtree - for simple spatial analysis
    8. pysal - advanced spatial analysis, coloring maps
    9. numpy - math library



## Installation (had so many errors - to be continued on day3)

1. Installing with Conda
a) Create a new conda environment and setup some configs
` conda create -n geo_env `
` conda activate geo_env `
` conda config --env --add channels conda-forge `
` conda config --env --set channel_priority strict `

b) install with conda
 ` conda install python=3 geopandas `
for mac follow  https://www.youtube.com/watch?v=9qxXk2JxsqA&list=PLewNEVDy7gq3DjrPDxGFLbHE4G2QWe8Qh&index=2
 ## Geospatial common datatypes

 1. Geospatial common datatypes
    -  common geospatial datatypes : Shapefile (.shp) and GeoJSON (geojson)

    - Shapefile is a vector data format that is developed and maintained mostly by a company called ESRI. It stores many important geospatial information including the topology, shape geometry, etc

    - GeoJSON, similar to JSON, stores geometry information (coordinates, projection, etc) in addition to your typical attributes relevant to the object (index, name, etc).

    - Once you load either of these dataformat using Geopandas, the library will create a DataFrame with the additional geometry column

- To understand basics take a look at basics.ipynb


