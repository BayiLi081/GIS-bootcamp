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



