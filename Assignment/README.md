# Assignment 1: Time Series Forecasting with ARIMA, Prophet, and LSTM

## 📌 Objective
The goal of this assignment is to apply three different time series forecasting models — *ARIMA, Prophet, and LSTM* — on a dataset and compare their performance. Finally, we decide which model works best for the given dataset.

---

## 📊 Dataset
- *Source:* Python built-in dataset (seaborn.load_dataset("flights"))  
- *Description:* Monthly number of airline passengers from *1949 to 1960*  
- *Columns:*
  - year → Year of observation
  - month → Month of observation
  - passengers → Number of airline passengers  
- Converted into time series format:
  - ds → Date (Year-Month combined)
  - y → Number of passengers

---

## 🔎 Steps I Followed
1. *Data Preprocessing*
   - Loaded the dataset using Seaborn.
   - Combined year and month into a single datetime column (ds).
   - Renamed columns to ds and y for Prophet compatibility.
   - Visualized the data to check *trend* and *seasonality*.

2. *ARIMA Model*
   - Checked stationarity of the series using Augmented Dickey-Fuller (ADF) test.
   - Differenced the data to make it stationary.
   - Selected parameters (p, d, q) using AutoARIMA.
   - Trained ARIMA and forecasted passenger numbers.

3. *Prophet Model*
   - Prepared dataset with ds and y.
   - Trained Prophet model and forecasted next 12 months.
   - Plotted *trend, yearly seasonality, and overall forecast*.

4. *LSTM Model*
   - Normalized the dataset (MinMax scaling).
   - Created sequences of past values to predict the next value.
   - Built and trained an LSTM neural network using Keras.
   - Forecasted future passenger numbers.

5. *Comparison*
   - Evaluated models using error metrics:
     - *RMSE (Root Mean Squared Error)*
     - *MAE (Mean Absolute Error)*
     - *MAPE (Mean Absolute Percentage Error)*
   - Compared forecast plots of each model with actual values.

---

## 📈 Results
- *ARIMA*  
  - Good at modeling the trend and seasonality.  
  - Requires careful tuning of parameters.  

- *Prophet*  
  - Very simple to use.  
  - Automatically handled yearly seasonality and trends.  
  - Clear interpretation of components (trend, seasonality, holidays).  

- *LSTM*  
  - Captured complex nonlinear patterns.  
  - Needed more data and computational time.  
  - Performance improves with larger datasets.  

---

## 📝 Learning
- Learned the difference between *statistical models (ARIMA, Prophet)* and *deep learning models (LSTM)* for time series forecasting.
- Understood that:
  - ARIMA is best for *small, stationary datasets*.  
  - Prophet is best for *business data with trend/seasonality/holidays*.  
  - LSTM is best for *large, complex datasets* with long-term dependencies.  

---

## ⚡ Conclusion
For this dataset (Airline Passengers), *Prophet worked the best* because:
- It captured both *trend* and *seasonality* automatically.  
- Easy to interpret and explain compared to ARIMA and LSTM.  
- ARIMA also worked well but needed more manual tuning.  
- LSTM was powerful but overkill for this small dataset.  

---
