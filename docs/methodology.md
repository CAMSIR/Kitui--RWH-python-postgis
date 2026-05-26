# Methodology

## Overview

This project applies GIS-based multi-criteria analysis to identify suitable areas for road water harvesting in Kitui County, Kenya. The workflow combines raster processing, vector processing, reclassification, and weighted overlay analysis.

## Study Area

The study area is Kitui County, Kenya. All spatial layers were processed and aligned to a common projected coordinate system, EPSG:32737, for consistent spatial analysis.

## Criteria Used

The suitability analysis used the following criteria:

- Rainfall
- Slope
- Soil type
- Soil depth
- Land cover
- Distance to roads
- Distance to agricultural areas

## Data Preparation

The datasets were prepared by:

1. Loading spatial datasets into Python
2. Checking coordinate reference systems
3. Reprojecting layers to EPSG:32737
4. Clipping or preparing layers for Kitui County
5. Reclassifying criteria into suitability scores
6. Aligning all rasters to a common 100 m grid

## Reclassification

Each criterion was reclassified into suitability scores from 1 to 5.

| Score | Suitability |
|---|---|
| 1 | Not suitable |
| 2 | Less suitable |
| 3 | Moderately suitable |
| 4 | Suitable |
| 5 | Highly suitable |

## Weighted Overlay

The reclassified criteria were combined using weighted overlay analysis. The initial weights used were:

| Criterion | Weight |
|---|---:|
| Rainfall | 0.25 |
| Slope | 0.20 |
| Soil type | 0.15 |
| Soil depth | 0.15 |
| Land cover | 0.10 |
| Distance to roads | 0.10 |
| Distance to agriculture | 0.05 |

The weighted overlay produced a continuous suitability raster, which was later classified into five final suitability classes.

## Final Output

The final output is a classified road water harvesting suitability map for Kitui County. The map identifies areas ranging from not suitable to highly suitable for road water harvesting implementation.