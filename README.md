# EDS220 Fall2021 Final Project 

## Los Angeles Tree Canopy Cover 

**Authors:**
Paloma Cartwright 
Mia Forsline
Halina Do-Linh 

**Intended Purpose:** 
This notebook is for educational purposes and the authors are Master of Environmental Data Science students from UCSB's Bren School of Environmental Science & Management. This repository is the final project for EDS 220: Remote Sensing and Environmental Data. The objective of the final project is to create a tutorial for fellow students based on any environmental data set. 

**Description:**
This notebook aims to explore the relationship between the percentage of modern tree canopy cover and historical 1939 redlining in Los Angeles County. To examine the link, we map the percentage of tree canopy cover in 2014, the grades assigned to residential areas by the federal government's Home Owners' Loan Corporation, and a composite map of both tree canopy cover and grades. We expect historical residential areas with the highest grade of A to demonstrate the highest percentage of modern tree canopy cover.

**Data:**
The data used is a combination of tree canopy data and land cover imagery data of LA County. Tree canopy data comes from [TreePeople](https://www.treepeople.org/), an environmental nonprofit that promote sustainable urban ecosystems, and the University of Vermont. The tree canopy data are a CSV file with polygon geometries from census tracts and tree canopy cover percentages for different census blocks. The Los Angeles Regional Imagery Acquisition Consortium (LARIAC) provided land cover 2014 imagery data obtained through aerial surveys. The land cover imagery data are shapefiles. We retrieved the data from the [County of Los Angeles Open Data](https://data.lacounty.gov/). One issue with this combined dataset is there is no descriptive metadata for the tree canopy data (i.e. no descriptions of variables). Metadata for the land cover 2014 imagery data can be found on [LARIAC's website](https://lariac-lacounty.hub.arcgis.com/pages/lariac5-documents-datahttps://lariac-lacounty.hub.arcgis.com/pages/lariac5-documents-data). Due to these issues, we focused on analyzing self-explanatory variables such as tree canopy (`'Can_P'`) and impervious surfaces (`'imperv_p'`). 

We also used data containing shapefiles of the Home Owners' Loan Corporation map for Los Angeles in 1939 illustrating the grades (A-D) for each neighborhood. We retrieved the data from the University of Richmond's [Mapping Inequality project](https://dsl.richmond.edu/panorama/redlining/#loc=5/39.1/-94.58&text=downloads). All of *Mapping Inequality*'s spatial, textual, and other data are licensed under a Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License. One issue with this dataset is that the historical spatial extent does not match up perfectly with modern LA County. There are a lot of gaps where the tree canopy cover and redlining data do not align, making it somewhat difficult to draw conclusions.

**Results:**
The results of this notebook provided a compostie map of LA County Tree Cover with Historical Redlining overlayed. Our target audience are LA policymakers and any stakeholders invovled in urban forestry. This data is particularly important for LA policymakers to consider since it has been found that tree canopy on residential parcels have been declining significantly since 1990 and we know that tree canopy provides numerous health and environmental benefits. Furthermore, this could help idenitify communities who need tree canopy the most, especially those who have been historically discriminated against.


**Contents:**
- data 
- la-tree-final-proj.ipynb: Completed notebook with working examples 
- la-tree-final-proj_blank.ipynb: Empty notebook for working through during the class presentation 
- environment.yml: Environment file for use in creating Binder environment for running Jupyter notebook

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/la-tree/notebook/HEAD)
