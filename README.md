

# AQI Prediction using SARIMA & LSTM

## Overview

This project aims to forecast **Air Quality Index (AQI)** using two powerful approaches: the **traditional time series model SARIMA** and the **deep learning model LSTM**. The historical AQI data is sourced from the **Central Pollution Control Board (CPCB)** to understand pollution patterns and make forward-looking predictions.

**Data Source:** [CPCB - Central Pollution Control Board](https://cpcb.nic.in/)

---

## Key Features

- Time series forecasting using SARIMA and LSTM  
- Preprocessing of raw AQI data and engineered time-based features  
- Seasonal and long-term AQI trend analysis  
- Visualization and comparative model evaluation  

---

## Tech Stack

| Category         | Tools and Libraries                        |
|------------------|---------------------------------------------|
| Programming      | Python                                      |
| Data Processing  | Pandas, NumPy                               |
| Time Series      | Statsmodels (SARIMA), TensorFlow/Keras (LSTM) |
| Visualization    | Matplotlib, Seaborn, Plotly                |

---

## Project Workflow

### 1. Data Preprocessing

- **Missing Data Handling:** Spline interpolation was used to fill missing AQI values.  
- **Date Feature Extraction:** Month, day, and hour were extracted from datetime columns.  
- **Normalization:** Applied scaling techniques for LSTM input.  
- **Outlier Detection:** Used statistical thresholds to identify and remove anomalies.

### 2. Time Series Modeling

#### SARIMA

- Designed to capture trend, seasonality, and noise.
- Utilized ACF and PACF plots for parameter selection.
- Differencing used to ensure data stationarity.
- Generated AQI forecasts based on seasonal trends.

#### LSTM

- Built using stacked LSTM layers to capture temporal dependencies.
- Employed a sliding window approach to create sequences.
- Trained on historical AQI data and compared results with SARIMA.

### 3. Model Evaluation

- **Metrics Used:** RMSE (Root Mean Squared Error), MAE (Mean Absolute Error), and MAPE (Mean Absolute Percentage Error).  
- **Insights Extracted:** Identified AQI variations across different seasons and timeframes.  
- **Model Comparison:** Assessed forecasting capabilities of both SARIMA and LSTM to determine effectiveness.

---

## How to Run

1. Download the AQI dataset from the [CPCB website](https://cpcb.nic.in/).
2. Open and run `data_preprocessing.ipynb` to clean and prepare the data.
3. Run `sarima_model.ipynb` to apply SARIMA for forecasting.
4. Run `lstm_model.ipynb` to use LSTM for AQI prediction.
5. Compare outputs from both models and visualize results.

---

## Future Enhancements

- Integrate additional variables such as weather, traffic, and industrial emission data for improved forecasting.  
- Optimize model parameters using grid/random search.  
- Develop and deploy an API for real-time AQI prediction.  
- Connect the model to live sensor networks for dynamic updates.

---

## Conclusion

This project delivers a dual-model framework for AQI forecasting using both traditional and deep learning approaches. It serves as a foundation for building more advanced, real-time air quality monitoring systems that support sustainable environmental policies and urban development planning.

---

## References

- [CPCB AQI Data](https://cpcb.nic.in/)
- [Pandas Documentation](https://pandas.pydata.org/)
- [Matplotlib Documentation](https://matplotlib.org/)
- [Statsmodels - SARIMA](https://www.statsmodels.org/)
- [TensorFlow/Keras](https://www.tensorflow.org/)

