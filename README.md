
# Analysis of MPG Dataset

## Introduction
This repository contains Python code for analyzing the MPG dataset. The dataset consists of information about various cars, including their miles per gallon (mpg), number of cylinders, displacement, horsepower, weight, acceleration, model year, origin, and car name.

## Importing Packages
The analysis is performed using several Python libraries:
- pandas: for data manipulation and analysis
- matplotlib.pyplot: for creating visualizations
- seaborn: for creating more complex visualizations
- statsmodels.api: for statistical analysis

## Initial Data Exploration
The code reads the dataset (`MPG.csv`) into a pandas DataFrame and displays the initial columns using `df.head()`.

## Data Preprocessing
- The 'horsepower' column is converted to numeric values, and rows with missing 'horsepower' values are dropped.
- Column names are standardized by renaming 'model year' to 'model_year' and 'car name' to 'car_name'.

## Exploratory Data Analysis (EDA)
The code provides various visualizations to explore the dataset:
- Histograms of 'mpg' and 'horsepower'
- Box plots of 'horsepower' and 'mpg' by 'origin'
- Scatter plots of 'mpg' vs. 'weight', 'mpg' vs. 'model_year', 'mpg' vs. 'cylinders', and 'mpg' vs. 'horsepower'
- Bar plots of 'mpg' by 'model_year' and 'cylinders'
- Joint plot of 'horsepower' vs. 'mpg'

## Linear Regression Models
Three linear regression models are built to predict 'mpg':
1. Model 1: Using only 'weight' to predict 'mpg'
3. Model 2: Using 'weight' and 'cylinders' to predict 'mpg'
4. Model 3: Using 'weight', 'cylinders', and 'horsepower' to predict 'mpg'

## Testing with Assumptions
A two-sample t-test is performed to test for a significant difference in 'mpg' between cars manufactured in the USA and Europe. The test results indicate a significant difference in 'mpg' based on the origin of manufacture.

## Conclusion
The analysis provides insights into the relationship between various factors and 'mpg' in the dataset.
