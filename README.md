# Time-Series Modeling & ARIMA-Based Forecasting of Electricity Load and Solar Generation

This project performs an end-to-end statistical time-series analysis and forecasting of electricity load and solar generation using classical ARIMA models. The objective is to study temporal dependency, stationarity, and forecast performance using rigorous statistical validation.

---

## Objective
- Analyze historical electricity load and solar generation patterns
- Test stationarity using the Augmented Dickey-Fuller (ADF) test
- Identify temporal dependence using ACF and PACF plots
- Build ARIMA models for short-term forecasting
- Evaluate predictive accuracy using Root Mean Squared Error (RMSE)
- Visually compare actual vs predicted values

---

## Dataset Description
- Time-indexed electricity system data with:
  - `utc_timestamp` – hourly timestamps
  - `IT_load_new` – electricity demand/load values
  - `IT_solar_generation` – solar power generation values
- Missing values handled using forward-fill methods
- Data transformed into time-series format for modeling

---

## Tools & Libraries
- Python
- Pandas, NumPy
- Matplotlib
- Statsmodels
- Scikit-learn

---

## Methodology
1. Converted timestamps to datetime format and visualized load and solar generation trends  
2. Handled missing values using forward-fill imputation  
3. Conducted stationarity testing using the AugFmented Dickey-Fuller (ADF) test  
4. Analyzed ACF and PACF plots to determine ARIMA parameters  
5. Performed time-based 80:20 train–test split  
6. Built ARIMA(2,0,2) models for:
   - Electricity load forecasting
   - Solar generation forecasting  
7. Evaluated model performance using RMSE  
8. Visualized actual vs predicted demand and generation outputs  

---

## Model Evaluation
- **Electricity Load Forecast RMSE:** ~7715  
- **Solar Generation Forecast RMSE:** ~2486  
- Forecast plots demonstrate that the ARIMA model captures the overall temporal structure and demand–generation trends with reasonable accuracy.

---

## Key Learnings
- Practical application of Augmented Dickey-Fuller stationarity testing
- Interpretation of ACF and PACF for ARIMA order selection
- End-to-end ARIMA model implementation for real energy system data
- Understanding forecast error behavior using RMSE
- Time-based validation of forecasting models

---

## Applications
- Power demand forecasting
- Renewable energy integration analysis
- Short-term load monitoring
- Statistical forecasting for economic and financial time-series

---

