# Los Angeles Tree Canopy Cover & Historical Redlining Visualization Analysis

## EDS 220: Remote Sensing and Environmental Data
## Fall 2021 Final Project 
### Due 2021-12-08

**Student Authors:**
- [Paloma Cartwright](palomacartwright@bren.ucsb.edu), UCSB
- [Mia Forsline](mforsline@bren.ucsb.edu), UCSB
- [Halina Do-Linh](hdolinh@bren.ucsb.edu), UCSB

### **Intended Purpose** 
This notebook is for educational purposes and the authors are [Master of Environmental Data Science](https://bren.ucsb.edu/masters-programs/master-environmental-data-science) students from UCSB's Bren School of Environmental Science & Management. This repository contains the final project for the courses EDS 220 (Remote Sensing and Environmental Data) and EDS 211 (Team Science, Collaborative Analysis, and Project Management). 

### **Project Motivation and Objective**
Our final project explores the relationship between the percent of modern tree canopy cover and historical 1939 redlining in Los Angeles County. This analysis is one way to acknowledge and think about the environmentally unjust history and its present-day ramifications in Los Angeles County. To do so, we map the percentage of tree canopy cover in 2014, the grades assigned to residential areas by the federal government's Home Owners' Loan Corporation (HOLC), and a composite map of both tree canopy cover and the HOLC grades. We expect historical residential areas with the highest grade of A to demonstrate the highest percentage of modern tree canopy cover. 

For this analysis we used the following packages: 
- `geopandas`
- `pandas`
- `matplotlib.pyplot`
- `cartopy.crs`
- `contextily`

### **Data**
The data used is a combination of tree canopy data and land cover imagery data of LA County. Tree canopy data comes from [TreePeople](https://www.treepeople.org/), an environmental nonprofit that promote sustainable urban ecosystems, and the University of Vermont. The tree canopy data are within a CSV file with polygon geometries from census tracts and tree canopy cover percentages for different census blocks. The Los Angeles Regional Imagery Acquisition Consortium (LARIAC) provided land cover 2014 imagery data obtained through aerial surveys. The land cover imagery data are shapefiles. We retrieved the data from the [County of Los Angeles Open Data](https://data.lacounty.gov/). We focused on analyzing the tree canopy (`'Can_P'`) and impervious surfaces (`'imperv_p'`) variables. 

We also used data containing shapefiles of the Home Owners' Loan Corporation map for Los Angeles in 1939 illustrating the grades (A-D) for each neighborhood. We retrieved the data from the University of Richmond's [Mapping Inequality project](https://dsl.richmond.edu/panorama/redlining/#loc=5/39.1/-94.58&text=downloads). All of *Mapping Inequality*'s spatial, textual, and other data are licensed under a Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License. 

### **Results**
We created a composite map of Los Angeles County's tree canopy cover overlaid with historical redlining grades. Our target audience are LA policymakers and stakeholders invovled in urban forestry. This data is particularly important for LA policymakers to consider since tree canopy on residential parcels has been declining significantly since 1990, and we know that tree canopy provides numerous health and environmental benefits. Furthermore, these findings could help idenitify vulnerable communities who could benefit the most from tree canopy, especially communities that have been historically discriminated against.


### **Contents**
- data 
- la-tree-final-proj.ipynb (Completed notebook with working examples)
- la-tree-final-proj_blank.ipynb (Empty notebook for teaching purposes)
- environment.yml (Environment file for use in creating Binder environment for running Jupyter notebook)

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/la-tree/notebook/HEAD)

↑↑↑↑↑↑↑↑↑↑↑↑↑↑↑ click the binder icon above to begin. A remote python session will launch in your browser with the tutorial. Be patient, sometimes it takes a while for the session to initalize the first few times.
