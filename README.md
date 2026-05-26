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


##  Outputs

The project has produced a final road water harvesting suitability raster for Kitui County using an AHP-based weighted overlay approach. The final suitability map combines rainfall, slope, land cover, soil depth, soil type, distance to roads, and distance to agricultural areas.

The final suitability classes are:

| Class | Suitability |
|---|---|
| 1 | Not suitable |
| 2 | Less suitable |
| 3 | Moderately suitable |
| 4 | Suitable |
| 5 | Highly suitable |

![Final Suitability Map](outputs/maps/kitui_rwh_final_suitability_map.png)