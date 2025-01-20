# Electricity Demand Forecast in Finland

This repository contains the group project report and related files for forecasting daily electricity consumption in Finland. The project was completed as part of an academic assignment.

## Overview

The goal of the project was to develop a model to forecast daily logarithmic electricity consumption in Finland, based on historical data and temperature readings from three cities: Helsinki, Tampere, and Rovaniemi. The forecasts were made for three specific days in March 2024 using an iterative approach to refine the models.

## Data Sources

- **Electricity Consumption**: Hourly electricity usage in Finland.
- **Temperature Data**: Hourly temperature readings from Helsinki, Tampere, and Rovaniemi.

## Methodology

### Data Preprocessing
- Addressed missing and outlier data points.
- Corrected time zone inconsistencies between data sources.
- Calculated daily averages for temperatures and summed hourly electricity consumption.

### Models Developed
1. **Linear Regression**: Initial exploration but showed strong autocorrelation in residuals.
2. **Holt’s Winter Methods**: Improved seasonality tracking but lacked robust variance modeling.
3. **Dynamic Regression with ARIMA**:
   - Incorporated temperature data, seasonality predictors, and Fourier terms for cyclic patterns.
   - Adjusted over three forecasting rounds to improve accuracy.

## Results

The model was refined over three rounds:
- **Round 1**: Dynamic regression with AIC = -6656.42.
- **Round 2**: Addressed data issues, AIC improved to -6669.03.
- **Round 3**: Added COVID-19 indicators and Fourier terms, achieving AIC = -6800.35.

## Key Findings
- Temperature and seasonality significantly influenced electricity demand.
- The final model achieved the lowest AIC, indicating improved model quality. However, simpler models (e.g., M2 in Round 3) may be more practical for resource-constrained scenarios.

## Limitations
- Models were limited by available data and scope.
- Further improvements could integrate additional predictors and domain expertise.

## Usage
This repository contains:
- The detailed project report (`Forecast_Report.pdf`).
- Data processing and modeling scripts.
- Forecast results for the specified dates.

## Acknowledgments
This work was completed as part of a course project at Aalto University, Finland. 
