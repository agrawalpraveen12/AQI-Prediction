# 🌍 AQI Prediction using SARIMA & LSTM

## 📌 Project Overview
This project focuses on **predicting Air Quality Index (AQI)** using **time series forecasting models**. The dataset is sourced from the **Central Pollution Control Board (CPCB)**, and the objective is to analyze historical AQI data, preprocess it, and apply machine learning techniques like **SARIMA** and **LSTM** for accurate AQI forecasting.

🔗 **Data Source:** [Central Pollution Control Board (CPCB)](https://cpcb.nic.in/)

---
## 🎯 Features
✅ Data cleaning and preprocessing for AQI analysis  
✅ Time series forecasting using **SARIMA** and **LSTM**  
✅ Visualization of AQI trends and seasonal variations  
✅ Model evaluation and performance comparison  

---
## 🛠️ Technologies Used
- 🐍 Python
- 📊 Pandas, NumPy
- 📉 Statsmodels (SARIMA), TensorFlow/Keras (LSTM)
- 📈 Matplotlib, Seaborn, Plotly

---
## 🔍 Techniques Used

### 1️⃣ Data Cleaning & Preprocessing
🛠️ **Handling Missing Values:** Used **Spline Interpolation** to fill missing AQI values smoothly  
📊 **Feature Engineering:** Extracted useful features from timestamps, such as month, day, and hour  
📆 **Datetime Conversion:** Converted date columns into proper datetime format for time series analysis  
📉 **Outlier Removal:** Identified and removed anomalies in AQI values using statistical methods  
📊 **Scaling & Normalization:** Standardized AQI values for improved model performance  

### 2️⃣ Time Series Forecasting Models

#### **SARIMA (Seasonal AutoRegressive Integrated Moving Average)**
🔄 Applied **SARIMA** to capture seasonality and trends in AQI data  
📊 Used **ACF & PACF** plots to determine optimal SARIMA parameters  
📉 Differenced data to ensure stationarity for accurate forecasting  
📈 Forecasted AQI for future time periods using SARIMA's seasonal components  

#### **LSTM (Long Short-Term Memory Networks)**
🤖 Built an **LSTM-based deep learning model** to learn AQI patterns from historical data  
📊 Applied **sliding window technique** to prepare time series sequences for training  
🧠 Used **multiple LSTM layers** to capture complex temporal dependencies  
📉 Compared LSTM predictions with SARIMA to evaluate deep learning model effectiveness  

### 3️⃣ Model Evaluation & Insights
📊 **Performance Metrics:** Evaluated forecasting accuracy using RMSE, MAE, and MAPE  
📌 **Trend Analysis:** Identified seasonal, monthly, and yearly AQI variations  
📈 **Model Comparison:** Compared **SARIMA vs. LSTM** performance to determine the best forecasting model  

---
## 🚀 How to Use
1️⃣ Load the dataset from **CPCB**  
2️⃣ Run the **data cleaning notebook** to preprocess the AQI data, including handling missing values and feature engineering  
3️⃣ Execute the **SARIMA model notebook** to generate AQI forecasts using classical time series analysis  
4️⃣ Run the **LSTM model notebook** to apply deep learning techniques for AQI prediction  
5️⃣ Compare the results from both models and analyze forecasting accuracy  

---
## 🔮 Future Enhancements
📢 **Incorporate Additional Factors:** Use weather, traffic, and industrial emissions data for improved predictions  
📊 **Hyperparameter Optimization:** Tune SARIMA and LSTM models for enhanced accuracy  
📡 **Real-time AQI Prediction:** Deploy as an API for live air quality forecasting  
🛰️ **Integration with IoT Sensors:** Collect real-time pollution data from smart sensors to improve predictions  

---
## 📌 Conclusion
This project provides a **data-driven approach to AQI forecasting** using **SARIMA and LSTM models**. By leveraging time series analysis and deep learning, we can predict air quality trends, aiding in pollution control measures and policy decisions.

---
## 📚 References
- CPCB AQI Data: [cpcb.nic.in](https://cpcb.nic.in/)
- Pandas: [pandas.pydata.org](https://pandas.pydata.org/)
- Matplotlib: [matplotlib.org](https://matplotlib.org/)
- Statsmodels (SARIMA): [statsmodels.org](https://www.statsmodels.org/)
- TensorFlow/Keras (LSTM): [tensorflow.org](https://www.tensorflow.org/)

