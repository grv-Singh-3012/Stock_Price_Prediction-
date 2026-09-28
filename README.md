# 📈 Stock Price Prediction Using Time Series & Deep Learning

## 📌 Overview

This project implements multiple **Machine Learning, Deep Learning, and Time Series forecasting models** to predict stock prices using historical SPY ETF data.

The main objective is to compare traditional forecasting approaches with deep learning models and evaluate their performance using standard regression metrics.

Models implemented include:

- Naive Forecasting
- Moving Average
- ARIMA
- Linear Neural Network
- Dense Neural Network
- RNN
- LSTM
- CNN + RNN
- WaveNet-inspired CNN

---

## 🛠 Tech Stack

**Language:** Python

**Libraries & Frameworks:**

- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Statsmodels
- TensorFlow
- Keras
- yfinance

**Development Environment:**

- Jupyter Notebook
- Google Colab

---

## 📊 Dataset

Historical stock market data for the **SPDR S&P 500 ETF Trust (SPY)** is used for model training and evaluation.

The dataset contains:

- Open
- High
- Low
- Close
- Adjusted Close
- Volume

Historical market data can also be downloaded using the `yfinance` API.

The primary forecasting task is to predict the **next trading day's closing price** using historical closing prices.

---

## 🔄 Project Workflow

```text
Historical SPY Data
        |
        v
Data Cleaning
        |
        v
Data Preprocessing
        |
        v
Train / Validation / Test Split
        |
        v
Feature & Sequence Generation
        |
        v
Model Training
        |
        +----------------------+
        |                      |
        v                      v
Statistical Models       Deep Learning Models
        |                      |
 Naive / SMA / ARIMA    Dense / RNN / LSTM / CNN
        |                      |
        +----------+-----------+
                   |
                   v
            Model Evaluation
                   |
                   v
          Forecast Visualization
