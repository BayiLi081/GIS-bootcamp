# Setting up CRS in QGIS

Create a new project, save it on the drive, and name it as you like. 

Drag the [bus_stops_singapore.shp](../../../GIS-bootcamp_qgisfiles/data/bus_stops_singapore.shp) into the canvas of QGIS

# Extra intro of QGIS

Right click of the layer, open the "Layer Properties"

Go through the tabs under layer properties:

1. Information

   General

   Coordinate Reference System

   Fields

2. Source

   Layer name

   Data source encoding (Gibberish text due to )

   Assigned CRS (Layer CRS)

3. Symbology

   Where you can play the visualisation (colour, size, etc.)

4. Labels

5. Fields

   Attributes data model

6. Other tabs are not usually used, but you can play around upon yourself.

## Project the file to another CRS

The use of **Reproject layer** tool in QGIS

The [bus_stops_singapore.shp](../../../GIS-bootcamp_qgisfiles/data/bus_stops_singapore.shp) comes with 4326, try to project to 3857

