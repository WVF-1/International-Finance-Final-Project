# International Finance Final Project

## Overview

This project extends traditional international finance forecasting methods by using machine learning techniques to optimize prediction accuracy. Specifically, it determines the optimal number of quarterly lags (1-12 quarters) that minimize the standard deviation of spot rate predictions across multiple forecasting methodologies.

## Problem Statement

Traditional international finance models use various methods to predict future spot rates, but selecting the appropriate time lag for predictions is often arbitrary. This project systematically evaluates different lag periods to identify which produces the most reliable forecasts with the lowest standard deviation.

## Forecasting Methods Analyzed

The project evaluates the following spot rate prediction methodologies:

- **Nominal Appreciation**: Projects future rates based on historical appreciation patterns
- **Forward Rates**: Uses forward exchange rates as predictors of future spot rates
- **International Fisher Effect (IFE)**: Relates interest rate differentials to expected exchange rate changes
- **Relative Purchasing Power Parity (RPPP)**: Links inflation differentials to exchange rate movements
- **Regression Analysis**: Statistical modeling of exchange rate determinants

## Methodology

1. **Data Parsing**: Extracts prediction data from the original Excel-based international finance analysis
1. **Grid Search Optimization**: Systematically tests lag periods from 1 to 12 quarters for each forecasting method
1. **Performance Evaluation**: Calculates standard deviation of prediction errors for each lag period
1. **Optimal Lag Identification**: Determines which lag minimizes prediction variance for each method

## Key Features

- Automated data extraction from Excel-based finance models
- Comprehensive grid search across 12 different lag periods
- Comparative analysis of multiple international finance forecasting techniques
- Statistical identification of optimal forecasting horizons
- Reduction of prediction standard deviation through data-driven lag selection

## Results

The project identifies the optimal lag period for each forecasting method, enabling more reliable and consistent exchange rate predictions compared to using arbitrary or fixed time horizons.

## Technologies Used

- Python
- Pandas (data manipulation)
- NumPy (numerical computations)
- Scikit-learn (grid search and model evaluation)
- Excel parsing libraries

## Data

The project uses exchange rate and economic indicator data from an international finance course final project, including historical spot rates, forward rates, interest rates, and inflation data.

## Future Improvements

- Extend analysis to additional forecasting methods
- Test on multiple currency pairs
- Implement cross-validation for more robust lag selection
- Explore non-linear lag relationships

## Acknowledgments

This project was developed as an extension of coursework in International Finance, applying machine learning techniques to traditional finance problems.