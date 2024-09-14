# County Health Outcomes Analysis

## Overview

This repository contains an analysis of health outcomes across counties in the United States, specifically focusing on premature age-adjusted mortality and various health indicators. The analysis uses data from the County Health Rankings and Roadmaps (CHR&R) program, supported by the Robert Wood Johnson Foundation, to explore the relationship between health indicators and premature deaths.

## Project Files

- **`Shapefiles_Data.shp`**: Shapefile containing geographic data for U.S. counties. This file will be used to create interactive maps visualizing the health outcomes across different counties.

- **`CountyHealthCode.Rmd`**: R Markdown file that includes the analysis, data processing, and visualization code. 

- **`2018 County Health Ranking Data v2.xls`**: Excel file containing the health data used for analysis. This includes information on premature age-adjusted mortality and various health indicators across different counties.

## Data Description

The data analyzed in this study is sourced from County Health Rankings and Roadmaps (CHR&R), a program of the University of Wisconsin Population Health Institute. CHR&R, supported by the Robert Wood Johnson Foundation, provides data on various health indicators and outcomes for U.S. counties.

### Variables

- **Dependent Variable:**
  - **Premature Age-Adjusted Mortality**: Number of deaths of residents under age 75 per 100,000 people in the county.

- **Independent Variables:**
  - **Adult Smoking (%)**: Percentage of adults who smoke.
  - **Adult Obesity (%)**: Percentage of adults classified as obese.
  - **Physical Inactivity (%)**: Percentage of adults who are physically inactive.
  - **Poor Mental Health Days**: Number of days per month that individuals report poor mental health.
  - **Diabetics (%)**: Percentage of adults with diabetes.

## Methodology

1. **Data Integration**: The data from the Excel file is cleaned and merged with shapefile data using a left join on county names.

2. **Data Processing**:
   - Convert raw counts of premature deaths to a mortality rate per 100,000 people.
   - Convert diabetes data to a percentage for consistency with other health indicators.

3. **Exploratory Data Analysis**:
   - Visualize the relationship between the dependent variable and independent variables using scatter plots.
   - Compute correlation coefficients to assess pairwise relationships.

4. **Regression Analysis**:
   - Perform linear regression to analyze the relationship between premature age-adjusted mortality and the selected health indicators.
   - Evaluate the significance of each predictor and the overall model fit.

5. **Visualization**:
   - Use the shapefile data to create interactive maps that visualize the predictors and their effects on county-level health outcomes.

## Limitations

- **Time Frame**: The analysis is based on data collected from 2018 to 2020. The COVID-19 pandemic caused significant disruptions, which may affect the accuracy and relevance of the findings.
  
- **Self-Reported Data**: Some variables such as poor mental health days, smoking, and obesity are self-reported and may be subject to reporting bias.

- **Limited Predictors**: The analysis uses a limited number of predictors, which may not fully capture all factors influencing premature age-adjusted mortality.


