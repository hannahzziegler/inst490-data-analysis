# INST490 Capstone Data Analysis
## Generic Open Dataset Charter Project #1

## Overview
This repository contains scripts written in Python and R for data cleaning, standardization and visualization of law enforcement and demographic data from the Center for Policing Equity. This project was undertaken by the Generic Open Dataset Charter #1 for the spring 2024 INST490 capstone class at the University of Maryland. The scripts help organize and standardize various datasets such as shapefiles, American Community Survey (ACS) data, and police encounters reports from multiple metropolitan areas in the United States. The goal is to facilitate easier analysis and visualization of the data and better understand the files in the Center for Policing Equity’s collection to craft documentation for them.

## Python Script
#### <em>Libraries Used:</em> 
- os: For interacting with the operating system to create directories, list directory contents, etc.
- shutil: Used for file operations such as copying.
- folium: For creating interactive maps to visualize geographic data.
- geopandas (gpd): For working with geospatial data.
  <br><br>
  
### Functionality:
- Directory Structure Creation: Sets up a new repository structure to organize data into categorized folders.
- Data Standardization:
<ul>
<li>Shapefiles: Standardizes shapefile names and organizes them into the correct directories.</li>
<li>ACS Data: Cleans and moves ACS data files, standardizing names and structures for easier access and analysis.</li>
<li>Geospatial Visualization:</li>
<li>Reads and transforms shapefiles to a consistent coordinate reference system.</li>
<li>Plots shapefiles and overlays additional geospatial data using folium to produce interactive maps.</li>
  </ul>
  <br><br>
  
## R Script
#### <em>Libraries Used:</em> 
- tidyverse: A collection of R packages designed for data science.
- janitor: Provides simple functions for examining and cleaning dirty data.
- sf: Supports simple features for handling spatial data.
- tigris: Loads geographic boundary data.
- foreign: For reading data stored by other software.

### Functionality:
Data Cleaning:
- Cleans and standardizes vehicle stops and use of force data from different departments.
- Separates date and time, standardizes column names, and addresses missing data issues.
- Shapefile Visualization:
<ul><li>Visualizes geographic boundaries of police jurisdictions.</li>
<li>Uses sf package to read and plot shapefiles, ensuring the data represents the correct geographic areas.</li></ul>

Handling ACS Data:
- Cleans and organizes ACS data, ensuring metadata is correctly associated with data files.

### Purpose of the Scripts
The scripts are designed to streamline the process of preparing the Center for Policing Equity’s data collection for analysis and documentation. By standardizing file names and structures, cleaning data and setting up directories in a consistent manner, these scripts make it easier to perform reproducible research and analysis on law enforcement data. These scripts also helped group members better understand the limitations and opportunities associated with working with this data collection, which contributed greatly to the final documentation the group created for other users to better understand these data files. 

### How to Use
Python Script: Ensure Python is installed, and run the script section by section to create directories, standardize files, and generate visualizations.
R Script: Open the R Markdown file in an R environment such as RStudio. Install the necessary packages and run the code chunks sequentially to process the data.
