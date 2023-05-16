# Calculating the NDVI in QGIS

## Download the Landsat 8 data

1. Create an account on [USGS](https://ers.cr.usgs.gov/register)
2. Login through the [username and password](https://ers.cr.usgs.gov/login)
3. Open [EarthExplorer](https://earthexplorer.usgs.gov/)
4. Type in **Landsat 8 (All matched results)** in Data Set Search
5. Ask Google/ChatGPT the difference between level 1 and level 2 data set, but in the study, we use the level 2 (overall, level 2 is more accurate)
6. Read the detail and information about the [USGS EROS Archive - Landsat Archives - Landsat 8-9 OLI/TIRS Collection 2 Level-2 Science Products | U.S. Geological Survey](https://www.usgs.gov/centers/eros/science/usgs-eros-archive-landsat-archives-landsat-8-9-olitirs-collection-2-level-2)
7. Read the [What are the band designations for the Landsat satellites? | U.S. Geological Survey (usgs.gov)](https://www.usgs.gov/faqs/what-are-band-designations-landsat-satellites)
8. Zoom to Singapore, and click **Use Map** (Or use the number of path and row of WRS: 125 and 059 in Additional Criteria)
9. Select the date range and choose the the data range you want to search (In this tutorial, we just limit to August in the search months box)
10. Limit the satellite to 8 in the additional criteria.

11. Limit the collection category to Tier 1

> What is the difference between Tier 1 and Tier 2 Landsat?
>
> **Tier 1 data have the highest radiometric and positional quality**. They have precision terrain processing and have been inter-calibrated across the Landsat sensors. The USGS recommends using Tier 1 data for all future time-series analysis. Tier 2 data are still very good images.

12. Show result
13. Use Browse overlay to double check that Singapore is covered
14. Then add the select date to bulk download (or open it and only download the band you want, in this case, band 4 and band 5 are what we are looking for)
15. Open item Basket and start order and submit
16. Later you will receive an email and download the data from the url enclosed

## Clip the file to the extent of Singapore

**Clip raster by extent**

Input Layer: for_CLIP.TIF

Clipping extent: Calculating from layer -> select the Singapore planning area layer

Clipped: Save to file -> Name it properly

**Clouds and cloud shadows?**

Clouds and cloud shadows can obscure the underlying surface features and can affect the accuracy of image analysis and interpretation.

There are algorithmns to mask out clouds in the satellite images different from products.

For example, in QGIS, you can follow [the tutorial to mask the clouds in Landsat 8 images](https://giscrack.com/application-of-masks-for-clouds-in-landsat-8-images-with-qgis/).

In this tutorial, we can just proceed to calculation as we only use the function of raster calculator.

## Conduct the Calculating

In **Landsat 8-9 Operational Land Imager (OLI) and Thermal Infrared Sensor (TIRS**):

| Bands                                | Wavelength (micrometers) | Resolution (meters) |
| ------------------------------------ | ------------------------ | ------------------- |
| Band 1 - Coastal aerosol             | 0.43-0.45                | 30                  |
| Band 2 - Blue                        | 0.45-0.51                | 30                  |
| Band 3 - Green                       | 0.53-0.59                | 30                  |
| Band 4 - **Red**                     | 0.64-0.67                | 30                  |
| Band 5 - **Near Infrared (NIR)**     | 0.85-0.88                | 30                  |
| Band 6 - Shortwave Infrared (SWIR) 1 | 1.57-1.65                | 30                  |
| Band 7 - Shortwave Infrared (SWIR) 2 | 2.11-2.29                | 30                  |
| Band 8 - Panchromatic                | 0.50-0.68                | 15                  |
| Band 9 - Cirrus                      | 1.36-1.38                | 30                  |
| Band 10 - Thermal Infrared (TIRS) 1  | 10.6-11.19               | 100                 |
| Band 11 - Thermal Infrared (TIRS) 2  | 11.50-12.51              | 100                 |

NDVI = (Band 5 – Band 4) / (Band 5 + Band 4)

```
(Singapore_20150820_B5@1 - Singapore_20150820_B4@1) / (Singapore_20150820_B5@1 + Singapore_20150820_B4@1)
```

Can manually type in or use the NDVI in predefined expressions

Reference Layer: use one of input layers

Change the symbology

| Bil  | Vegetation Classes | Description                               | NDVI Values  |
| ---- | ------------------ | ----------------------------------------- | ------------ |
| 1    | Non-Vegetation     | Barren areas, build up area, road network | -1 to 0.199  |
| 3    | Low Vegetation     | Shrub and grassland                       | 0.2 to 0.5   |
| 3    | High Vegetation    | Temperate and Tropical urban forest       | 0.501 to 1.0 |

Urban Vegetation Classes and NDVI value (Source: )