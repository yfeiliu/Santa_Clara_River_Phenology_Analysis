# Analyzing Plant Phenology Along the Santa Clara River using Landsat Imagery

## Overview

This project focuses on analyzing phenological patterns of different plant communities near the Santa Clara River, which flows from Santa Clarita to Ventura. We aim to investigate the phenological patterns of different plant communities, including riparian forests, grasslands, and chaparral shrublands, through a time series of Landsat imagery and polygons identifying the locations of study sites within each plant community.


## Data

- **Landsat Operational Land Imager (OLI sensor)**: Eight pre-processed scenes from 2018 to 2019 with spectral bands 2-7.
- **Study sites**: Polygons representing various plant communities tagged with one of the three plant types.

The dataset associated with this project is too large for direct inclusion in this GitHub repository. Please download the data from the provided [Google Drive link](https://drive.google.com/file/d/1e9ZwWoC6kmqy5r7WtDOkabYa02jMx_sd/view?usp=sharing) to replicate the analysis. Unzip the folder and all the contents and store in your directory as follows.

```         
Land_Cover_Classification_in_Santa_Barbara
│   .gitignore
│   README.md
│   Rmd/Proj files 
│
└───Report
    │   Santa_Clara_River_Phenology_Analysis.html
    │   Phenological_Trends.png
│
└───data
    │   study_sites.shp
    │   landsat_20180612.tif
    │   landsat_20180815.tif
    │   landsat_20181018.tif
    │   landsat_20181103.tif
    │   landsat_20190122.tif
    │   landsat_20190223.tif
    │   landsat_20190412.tif
    │   landsat_20190701.tif
                
```

## Getting Started

1. **Clone the Repository**: Clone or download this repository to your local computer.
2. **Date Setup**: Download the data from the above link and place it in the `data` directory.
3. **Run the Analysis**: Open the R Markdown files in the `Rmd/Proj files` directory to view and run the analysis. Ensure you have installed all necessary R packages.


## Analysis Overview

The R Markdown files contain a detailed breakdown of the analysis process, including:

1. **Converting Spectral Reflectance to NDVI**: Transforming spectral reflectance data from Landsat imagery into Normalized Difference Vegetation Index (NDVI) to measure vegetation productivity.
2. **Annual NDVI Calculation**: Computing NDVI for multiple time points throughout the year to capture seasonal variations in vegetation.
3. **NDVI Summary within Vegetation Communities**: Aggregating NDVI values for different vegetation communities to understand distinct phenological patterns.
4. **Visualization of NDVI Variations**: Creating graphical representations to illustrate temporal changes in NDVI across various vegetation types.

## Visualizing Phenological Trends
Visualization of the seasonal changes in NDVI across the different vegetation types.
![Phenological Trends](Phenological_Trends.png)