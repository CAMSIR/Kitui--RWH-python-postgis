# Kitui county Road water harvesting Suitability Mapping
This project focuses on identifying sites for rain water haversting along the road  in Kitui county,Kenya.

-python
-GeoPandas
-Rasterio
-PostGIS
-GIS-based Multi-Criteria Analysis

## Objectives
-prepare spatial datasets
-process road networks
-Analyse runoff potential
-Generate Suitability maps

## Study Area
Kitui County,Kenya

## Tools and Technologies
-python
-QGIS
-postGIS
-Jupyter notebook
-VS Code

## Raster data processing
Raster datasets are prepared by checking their coordinate reference systems,clipping them to the Kitui county boundary and
rprojecting them to EPSG:32737'
The raster layers used in this project include DEM,rainfall,LULC,soil depth and other suitability criteria.
The proccesed raster layers will be used to derive slope,create suitability classes and support the weighted overlay analysis for road water harvesting selection.

## Current Progress
-Repository created
-Kenya count adminstrative boundaries created
-Kitui boundary extracted
-Road data processing ongoing
-soil data clippedto Kitui county