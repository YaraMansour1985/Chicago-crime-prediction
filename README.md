# Chicago-crime-prediction
## Project Overview
This project focuses on analyzing and forecasting crime patterns in Chicago using *time series forecasting techniques*.  
Historical crime data is studied to understand trends, seasonality, and future crime behavior.

The main goal is to build reliable forecasting models that can help understand how crime rates evolve over time.

---

## Objectives
- Analyze historical Chicago crime data
- Check stationarity of the time series
- Identify trends and seasonality
- Build and compare *ARIMA* and *SARIMA* models
- Forecast crime rates for future periods
- Evaluate model performance using statistical metrics

---

## Dataset
- The dataset contains historical crime records for the city of Chicago.
- The date column was used as the time index.
- Data was aggregated over time to form a time series suitable for forecasting.

---

## Methodology

### 1. Data Preprocessing
- Converted date column to datetime format
- Set date as the time series index
- Handled missing values
- Aggregated crime counts over time

### 2. Stationarity Check
- Visual inspection of the time series
- Rolling mean and rolling variance
- Augmented Dickey-Fuller (ADF) test
- Differencing applied to make the series stationary

---

### 3. ARIMA Model
- Identified parameters *(p, d, q)* using:
  - ACF (Autocorrelation Function)
  - PACF (Partial Autocorrelation Function)
- Built ARIMA model
- Evaluated using AIC and BIC
- Generated forecasts

---

### 4. SARIMA Model
- Extended ARIMA to handle seasonality
- Identified seasonal parameters *(P, D, Q, s)*
- Captured weekly/monthly seasonal patterns
- Compared performance with ARIMA

---

## Model Evaluation
- AIC and BIC were used for model comparison
- Residual diagnostics were analyzed
- Forecast accuracy was evaluated using error metrics such as:
  - MAE
  - RMSE
  - MAPE

---

## Forecasting
- Future crime rates were forecasted for upcoming periods
- Forecast results were visualized alongside historical data
- Seasonal behavior was clearly captured using SARIMA

---

## Tools & Libraries
- Python
- Pandas
- NumPy
- Matplotlib
- Statsmodels
- Jupyter Notebook / Google Colab

---

## Results
- Both ARIMA and SARIMA models were successfully implemented
- SARIMA performed better when seasonality was present
- The models provided meaningful insights into crime trends in Chicago

---

## Conclusion
Time series models such as ARIMA and SARIMA are effective tools for crime trend analysis and forecasting.  
Incorporating seasonality significantly improves prediction accuracy for real-world crime data.

---

## Author
*Yara Mansour*

---

## Future Work
- Include external factors (weather, holidays, events)
- Try advanced models (Prophet, LSTM)
- Perform crime-type-specific forecasting
