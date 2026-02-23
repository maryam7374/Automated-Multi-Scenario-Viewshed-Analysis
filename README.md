# Automated-Multi-Scenario-Viewshed-Analysis

An automated and parameterized multi-scenario viewshed analysis workflow developed in ArcGIS Pro using ArcPy.

---

## Project Overview

This project was developed as a final course assignment.  
The main objective is to automate the viewshed analysis process in a structured and reusable way.

The notebook allows users to perform visibility analysis based on a Digital Elevation Model (DEM) and different observer heights.

---

## What This Notebook Does

This workflow performs the following steps:

1. Sets up the ArcGIS environment.
2. Allows the user to define the geodatabase workspace.
3. Lists available DEM rasters inside the geodatabase.
4. Lets the user select a DEM.
5. Generates a fishnet grid based on the DEM extent.
6. Converts grid cells into observer points.
7. Allows the user to define one or multiple observer heights.
8. Runs Viewshed2 analysis in FREQUENCY mode.
9. Saves each viewshed result separately.
10. Calculates basic visibility statistics for each scenario.

---

## Main Objective

The purpose of this project is to:

- Automate the viewshed analysis workflow
- Reduce manual geoprocessing steps
- Enable multi-height scenario comparison
- Improve clarity and reproducibility of spatial analysis

---

## Requirements

To run this notebook, you need:

- ArcGIS Pro
- Spatial Analyst extension
- A valid geodatabase
- At least one DEM raster stored inside the geodatabase

---

## How to Run

1. Open the notebook in ArcGIS Pro.
2. Enter the full path to your geodatabase.
3. Select a DEM from the available list.
4. Enter the desired grid spacing (in meters).
5. Enter one or multiple observer heights (comma separated).
6. Wait for the viewshed results and statistics.

Each height scenario produces:
- A separate viewshed raster
- Visibility percentage results printed in the console

---

## Example Applications

This workflow can be used for:

- Urban visibility studies
- Landscape planning
- Building height impact analysis
- Wind turbine siting
- General spatial visibility modeling

---

## Notes

- Processing time depends on DEM resolution and grid spacing.
- Smaller grid spacing increases computational cost.
- DEM resampling can be used to reduce processing time if needed.

---

## Author

Developed as part of a GIS course project using ArcPy automation.
