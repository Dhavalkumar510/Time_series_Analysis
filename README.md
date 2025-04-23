# 📈 Time Series Analysis of Johnson & Johnson Sales & Amazon Stock Price

## 🔍 Overview
This project applies time series forecasting on:

Johnson & Johnson: Quarterly sales data

Amazon: Daily stock prices (from Yahoo Finance)

We used both statistical (ARIMA) and deep learning (LSTM) models, along with Fourier filtering, to uncover trends and improve forecasting accuracy.

## 📁 Datasets
J&J Sales: Quarterly data over multiple years

Amazon Stock: Daily closing prices

## 🛠 Tools & Libraries
Python, pandas, numpy, matplotlib, statsmodels, pmdarima, scikit-learn, tensorflow/keras, scipy, seaborn

## 🔧 Methodology
EDA & Stationarity Testing

Time series plots

ADF test

Box-Cox Transformation

ACF & PACF Analysis

Informed ARIMA order selection

Modeling

ARIMA(6,1,3) (chosen via AIC) → 24-month forecast

LSTM → Scaled data, 60-step sequences, iterative forecasting

Butterworth Filter → Noise reduction via FFT

Evaluation

RMSE used for performance comparison

## 📊 Results

| Model | Dataset | RMSE  |
|-------|---------|-------|
| ARIMA | J&J     | -     |
| LSTM  | J&J     | 2.45  |
| LSTM  | Amazon  | 5.19  |

Forecast plots include confidence intervals (ARIMA)

## ✅ Conclusion
Combining ARIMA and LSTM improves accuracy. Key takeaways:

Stationarity & transformation are crucial

AIC & RMSE guide model selection

FFT filtering improves data quality

## 🔮 Future Work
Try SARIMA, Prophet

Add external factors (e.g., sentiment)

Explore ensemble forecasting

