# DSC530 Final Project

## Overview
This project analyzes various environmental variables to understand their distributions, relationships, and impacts on temperature. The analysis includes descriptive statistics, visualizations, outlier detection, and regression modeling.

## Data
The dataset used in this project is `climate_change.csv`, which contains the following environmental variables:
- Aerosols
- CH4 (Methane)
- MEI (Multivariate ENSO Index)
- CO2 (Carbon Dioxide)
- Temp (Temperature)

## Analysis

### Descriptive Statistics
Descriptive statistics provide insights into the central tendency, variability, and distribution of the environmental data. Key statistics include mean, mode, standard deviation, and skewness.

### Visualizations
Several visualizations are created to explore the data:
- Histograms: Show the distribution of each environmental variable.
- Scatter Plots: Illustrate the relationships between variables, such as CO2 vs. Temp, MEI vs. Temp, Aerosols vs. Temp, and CH4 vs. Temp.
- Cumulative Distribution Function (CDF): Displays the cumulative probability of CO2 concentrations.

### Outlier Detection
Outliers are identified using the Z-score test. Data points with Z-scores beyond a threshold (e.g., 3 standard deviations) are considered outliers and are removed from the dataset.

### Regression Modeling
A multiple linear regression model is built to predict temperature (Temp) based on CO2, Aerosols, and MEI. The model's performance is evaluated using R-squared, adjusted R-squared, and other statistical metrics.

## Key Findings
- Aerosols exhibit a left-skewed distribution, while CH4 shows a right-skewed distribution.
- CO2 displays an inverted U-shaped distribution, and temperature has a slight double-peaked distribution.
- The regression model indicates that CO2, Aerosols, and MEI significantly impact temperature, with CO2 having a positive correlation and Aerosols having a negative correlation.

## Usage
To run the analysis, execute the Jupyter Notebook `src/Schincke_DSC530_FinalProject.ipynb`. Ensure you have the necessary libraries installed:
- pandas
- seaborn
- statsmodels
- numpy
- scipy
- matplotlib

You can install these libraries using pip:
```sh
pip install pandas seaborn statsmodels numpy scipy matplotlib