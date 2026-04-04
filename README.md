# Lidar Forest Analysis

This is a workflow for generating lidar-derived forest products and modeling key forest attributes.

## Overview

Using discrete-return lidar data, this project:

* Generates terrain and canopy surface models
* Extracts plot-level lidar metrics
* Builds statistical models to predict forest attributes
* Produces wall-to-wall spatial predictions

## Outputs

* Digital Elevation Model (DEM)
* Canopy Height Model (CHM)
* Total Above-Ground Biomass (AGB)
* Dominant Tree Height maps

## Methods

* Point cloud filtering and preprocessing
* Raster generation at 2 m resolution
* Metric extraction from plot locations
* Forward variable selection for model development
* Linear modeling and performance evaluation (R²)

## Data

* 24 `.las` lidar tiles (~3 returns/m²)
* Plot data including location, AGB, and dominant height

## R Packages

* `lidR`, `terra`, `sf`, `dplyr`, `ggplot2`


## Notes

* Points below 0 m and above 55 m are filtered out
* Ensure variables used in models are not highly correlated

---
