# Used Car Price Prediction
Machine Learning project using Linear Regression to predict used car prices following the CRISP-DM framework.

## Project Overview

This project develops a machine learning model to predict used car prices using a dataset of vehicle listings. The project follows the CRISP-DM framework, including Business Understanding, Data Understanding, Data Preparation, Modeling, Evaluation, and Deployment.

The primary objective is to identify the factors that most strongly influence resale value and provide business recommendations for used car dealerships to improve pricing and inventory decisions.

## Business Problem
Used car dealerships must determine competitive yet profitable selling prices for vehicles while deciding which vehicles are worth purchasing.

This project builds a regression model capable of estimating vehicle prices based on characteristics such as:
- Vehicle age
- Mileage
- Manufacturer
- Condition
- Fuel type
- Transmission
- Drive type
- Vehicle type
- Title status
- Paint color
- State

## Dataset
Source: Craigslist Vehicles Dataset
Records after cleaning: 366,434
Target variable: Price

Features include:
- Age
- Odometer
- Manufacturer
- Condition
- Cylinders
- Fuel
- Transmission
- Drive
- Vehicle Type
- Paint Color
- State
- Title Status

## Data Preparation
The following preprocessing steps were performed:
- Removed missing values
- Removed invalid vehicle prices
- Converted Year into Vehicle Age
- Converted Cylinders into numerical values
- Ordinal encoded Vehicle Condition
- One-Hot Encoded categorical variables
- Standardized numerical variables
- Implemented preprocessing using Scikit-Learn Pipelines

## Models Evaluated
The Linear Regression model was selected because Ridge and Lasso regularization did not significantly improve predictive performance.

## Key Findings
The analysis suggests that:
- Vehicle age negatively impacts resale value.
- Higher mileage is associated with lower prices.
- Vehicle condition strongly influences price.
- Clean titles command higher resale values.
- Manufacturer is one of the strongest predictors of price.
- Trucks and pickup vehicles generally retain value better than several other vehicle types.

## Business Recommendations
Used car dealerships should:
- Prioritize lower-mileage vehicles.
- Purchase newer vehicles when possible.
- Focus on clean-title inventory.
- Invest in manufacturers with stronger resale value.
- Use the regression model as a pricing support tool rather than replacing expert judgment.
        
## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-Learn
- Jupyter Notebook
