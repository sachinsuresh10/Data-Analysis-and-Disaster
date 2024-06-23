# Data-Analysis-and-Disaster

## Overview

This project analyzes disaster data from the DesInventar database, focusing on various types of disasters and their impacts across different countries. The main sponsor of the database is the United Nations Office for Disaster Risk Reduction (UNDRR).

## Country List

Our group analyzed data for the following countries:
- Cambodia
- Ethiopia
- Ghana
- Indonesia
- Jordan
- Mali
- Morocco
- Mozambique
- Myanmar
- Nepal
- Niger
- Pakistan
- Iran

## Project Agenda

1. **Data Cleaning**
    - Removal of columns with all null values.
    - Removal of columns with 90% null data.
    - Merging of columns with similar combinations.
    - Categorization of events based on incidents.
    - Imputation using Random Forest Method.

2. **Data Visualization**
    - Bar Plots
    - Pie Charts
    - Donut Charts

3. **Regression Modelling**
    - Multi-linear regression and XGBoost models to predict losses (in USD) and deaths.

4. **Classification**
    - Classification of disasters by country and event type using:
        - Random Forest
        - K-Means
        - XGBoost

5. **Principal Component Analysis (PCA)**
    - Dimensionality reduction and data structure analysis.

## Data Pre-processing

The dataset was cleaned and pre-processed using R scripts. Missing values were imputed using the Random Forest method to enhance data completeness and reliability.

## Data Visualization

We created various plots to visualize the data, including:
- Bar graphs showing the frequency of deaths, injuries, and missing persons across different events.
- Bar graphs showing the number of events per decade.
- Area plots visualizing event combinations over the years.
- Pie and donut charts showing the distribution of infrastructure damage, deaths, and missing persons across Asia and Africa.

## Regression Modelling

- **Losses in USD**:
    - Multi-linear regression: Adjusted R² = 0.735
    - XGBoost: Adjusted R² = 0.8924

- **Deaths**:
    - Multi-linear regression: Adjusted R² = 0.5037
    - XGBoost: Adjusted R² = 0.720

## Classification Results

- **Country Prediction**:
    - Random Forest: Accuracy = 73.76%
    - K-Means: Accuracy = 5.56%
    - XGBoost: Accuracy = 86.2%

- **Event Type Prediction**:
    - Random Forest: Accuracy = 52.42%
    - K-Means: Accuracy = 13.20%
    - XGBoost: Accuracy = 98.86%

## Principal Component Analysis (PCA)

PCA was utilized to reduce the dimensionality of the numerical data, retaining significant information for further analysis and interpretation.

## Report

The full analysis and results are detailed in the accompanying [Report.pdf](Report.pdf).

## How to Run

1. **Data Download**:
    - Visit [DesInventar](https://www.desinventar.net/DesInventar/)
    - Select a country, go to the Statistics tab, choose Year/Month and Event, then download the data as an Excel or CSV file.

2. **Pre-processing and Analysis**:
    - Use the provided R scripts for data cleaning and imputation.
    - Use Python (with libraries like Pandas, Scikit-learn, XGBoost) for data visualization, regression, classification, and PCA.

## Dependencies

- R
- Python
- Pandas
- Scikit-learn
- XGBoost
- Matplotlib
- Seaborn

