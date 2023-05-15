# GIS Bootcamp for MUSPP students

Contributors: Li Bayi

## Preparation

In this bootcamp, QGIS will be used for several advantages:

- Open source
- Cross-Platform
- Integration with Python

Please make sure that you have properly installed the QGIS from the [official website](https://qgis.org/en/site/forusers/download.html) before the bootcamp started. You can download the LTR version as it is more stable to run on your computer and compatible to more extensions normally.

## Day 01

**00:00 - 00:15**: 

Software installation troubleshooting (QGIS)

**00:15 - 01:00**: 

- **15 mins**: [Introduction of GIS](http://www.bayi.in/GIS-bootcamp/#1)
- **15 mins**: The data model in GIS
  - mainly attribute data model
- **15 mins**: What is spatial data?
  - Concept
  - Entities and terms
  - Format: Raster verses Vector
  - [Spatial reference](./contents/spatial_reference/coordinatesystem.md)

**01:00 - 01:15**: 

Break and small Q&A

**01:15 - 02:00**:

- **10 mins**: [Introduction of spatial analysis](./contents/002_definespatialanalysis.md)
- **25 mins**: Spatial pattern
  - spatial pattern and the process created it
  - example of spatial analysis
  - common research questions related to spatial pattern investigation in urban research
- **10 mins**: Basic softwares and techniques for GIS
  - Open-source and close-source solutions
- **10 mins**: Q&A

**02:00 - 02:45**:

Common spatial analysis methods and their applications in urban research
- **15 mins**: [Spatial autocorrelation](./contents/spatialautocorrelation.md)
- **15 mins**: [Local Indicators of Spatial Association (LISA)](./contents/lisa.md)
- **15 mins**: [Global verses Local Statistics](./contents/globallocal.md)

**02:45 - 03:30**

**Practical**: [Create a map with essential elements in QGIS ](./contents/Practical01.md)

- 15 min: Short demonstration and hands-on practice
  - Download road network with QGIS plugin - QuickOSM


## Day 2

**00:00 - 01:00**:

**Practical**: "Where should I live in the city?" residence-selection analysis (network-based accessibility analysis)

[(PDF) Spatial Patterns for Crime Spots (researchgate.net)](https://www.researchgate.net/publication/330117670_Spatial_Patterns_for_Crime_Spots)

maybe replace it with crime spots analysis, residential choice model is way too complicated

- 30 min: Instruction and demonstration
- 30 min: hands-on practice

**01:00 - 01:15**: 

Break and small Q&A

**01:15 - 02:00**: Integration with [Remote sensing](./contents/rs.md)

- Introduction of remote sensing
  - Introduction
  - How could we apply remote sensing analysis in urban research?

- Common RS indexes and the calculation of them applied in urban research:

  - Normalized Difference Vegetation Index (NDVI)

  - Normalized Difference Built-up Index (NDBI)

  - Land Surface Temperature (LST)

**02:00 - 02:15**:

Break and small Q&A

**02:15 - 03:00**: 

- **10 mins**: Introduce some common data sources for remote sensing

- **Practical**: "Witness the climate change" spatiotemporal analysis on urban heat island
  - 30 min: Instruction and demonstration
  - 5 min: Q&A

Hands-on practice is required to complete after class and to be continued in next day's class.

## Day 03

**00:00 - 00:30**: 

Troubleshooting on yesterday's practical and explain the answer step by step

**00:30 - 01:00**: 

- **15 mins**: [Spatial Joins and data aggregation](./contents/overlay.md)
- **15 mins**: [Spatial interpolation](./contents/spatialinterpolation.md)

**01:00 -  01:10**: 

Break and small Q&A

**01:10 -  01:40**: 

- **15 mins**: Geocoding and address matching
- **15 mins**: Short demonstration of using Google Map API to translate address into coordinates

**01:40 -  01:50**: 

Break and small Q&A

**01:50 - 02:30**: 

Geospatial analysis and visualisation with other tools:

- **20 mins**: How to use the emerging technologies and tools in GIS to assist your research? 
  - light-coding problem solving skill
- **20 mins**: How to use Python scripts to power up your spatial analysis task in QGIS?
  - PyQGIS tutorial and basic demonstration

**02:30 -  03:00**: 

- **Practical**: "Do not recreating wheels!" using existing analysis pakage/API to perform analysis tasks in batch
  - **20 mins**: Demonstration
  - **20 mins**: Hands-on practice

**03:00 - 03:30**: Open discussion on career opportunities in the cross field and Q&A
