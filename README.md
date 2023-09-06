# US Home Price Prediction Model

## Overview
This repository contains code for building and analyzing a Lasso Regression model to predict US home prices using supply and demand factors as features. The model aims to explain how these factors have impacted home prices over the last 20 years.

## Data Sources
The data used in this project is sourced from the following files:
- `supply_data.csv`: Data related to supply-side factors.
- `demand_data.csv`: Data related to demand-side factors.
- `CSUSHPISA.csv`: S&P Case-Schiller Home Price Index data as a proxy for home prices.

## Data Preprocessing
- The data is preprocessed using the `data_preprocessing` function to:
  - Standardize date formats for merging datasets.
  - Merge supply and demand datasets based on date.
  - Remove unnecessary columns.

## Exploratory Data Analysis (EDA)
- EDA includes visualizations of:
  - Distribution of individual features.
  - Scatter plots showing the relationship between features and CSUSHPISA.
  - A heatmap displaying feature correlations.

## Lasso Regression Model
- The Lasso Regression model is built to predict CSUSHPISA based on supply and demand features.
- Model performance is evaluated using Mean Squared Error (MSE) and R-squared (R2) scores.
- Predicted CSUSHPISA values are plotted over the years.

## Model Analytics
- A scatter plot compares actual CSUSHPISA values (Y_test) with predicted values (y_pred).
- A histogram of residuals (prediction errors) is plotted to visualize the error distribution.

## Dependencies
- Python 3.x
- Libraries: pandas, numpy, scikit-learn, matplotlib, seaborn

## Usage
1. Clone the repository.
2. Install the required dependencies.
3. Run the Jupyter Notebook or Python script to execute the code.
