# Global Sugar Prices Forecasting
Using R, cleaned, transformed, and decomposed historical sugar price data to build forecasts supporting procurement timing and risk reduction decisions.

**Goal:** Give supply chain procurement teams for companies in the United States advice on purchasing sugar inventory for the next 2 years based on a simple forecast.

**Dataset Overview:**
- Dataset from FRED ( https://fred.stlouisfed.org/series/PSUGAISAUSDM )
- Global Sugar Prices from January 1, 1990, to January 1, 2025 - Monthly frequency
- Key columns:
  - observation_date --> Daily observation date
  - PSUGAISAUSDM --> Price of Sugar in Cents per U.S. Pound
  - dt --> Daily observation date in date format (created column)
  - rm --> Rolling Average of data set (created column)
  - rsd --> Rolling standard deviation (created column) 

**Project Components:**  
  1. Introduction
     - Describe the dataset 
  2. Data Cleaning
     - Clean the data by checking for missing values, duplicates, and outliers, and handling as necessary
  3. Data Understanding
     - Understand the dataset by making observations through a regular timeseries, moving average, moving standard deviation, and seasonal plot
  4. Data Transformation & Decomposition
     - Apply transformations and decomposition data for further understanding
  5. Forecasting Models
      - Implement 3 forecasting models and choose the best fit with accuracy metrics (RMSE, MAE, MAPE) and information criteria (AIC, AICc, BIC)
  6. Real World Interpretations
      - Translated forecast results into practical recommendations for procurement planning and risk management

**Tools & Techniques:**
- Tools: R (ggplot2, tseries, zoo, forecast)
- Techniques: Residual diagnostics, STL decomposition, Naïve, ARIMA, ETS, Model Diagnostics

**Recommendations:**  
- Because forecasted sugar prices are very uncertain, procurement teams should diversify suppliers and ensure flexible contracts are created
- Safety stock should be purchased, preferably around late August to early September, to avoid paying peak sugar prices
