# Create a map with essential elements in QGIS

## Download road network with QGIS plugin - QuickOSM

### Install QuickOSM through the plugin manager

1. Plugins - Manage and install plugins
2. Key in "QuickOSM"
3. "install plugin"
4. Two buttons of QuickOSM will be displayed in the top panel of main window

### Download the data

Click the QuickOSM button (green one) or go to Vector - QuickOSM - QuickOSM

1. Select which entities you want to query from OSM database

```sql
"highway" = 'primary' OR "highway" = 'road' OR "highway" = 'secondary'
```

Detail about key-value pairs used in OSM can read from [OSM wiki: Key:highway](https://wiki.openstreetmap.org/wiki/Key:highway)

2. Select the spatial extent of the data
3. Run query

It should take a while to acquire the data depending on the scale of query.

### Add point feature by coordinates

1. Go to Google Map, find the location you want to add, and  find its coordinates (longitude and latitude)
2. Create a point format vector layer, 

,1.3534019156675352

103.94455612645753

## Basic Elements of a Map

1. Title: 

   A concise and descriptive title that summarizes the main theme or purpose of the map.

2. Legend or Key:

   A legend or key that explains the symbols, colors, and other features on the map and their meaning.

3. Scale: 

   A scale that shows the relationship between the distances on the map and the actual distances on the Earth's surface.

4. North arrow or compass rose: 

   A north arrow or compass rose that indicates the orientation of the map and helps the reader to identify the cardinal directions (north, south, east, and west).

Additions:

1. Data sources:

   A statement that identifies the sources of data used to create the map, including the date of data collection and the method used to obtain the data.

2. Projection:

   A projection that shows how the three-dimensional Earth is represented on a two-dimensional surface and helps to minimize distortion of geographic features.

3. Insets or Overview map:

   Insets or overview maps that provide additional information about a specific area or the larger context of the map.
