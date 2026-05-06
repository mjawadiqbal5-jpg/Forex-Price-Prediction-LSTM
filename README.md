# Multivariate Forex Forecasting Engine: GBP to BDT

An advanced machine learning project using **Deep Learning (LSTM)** to project currency exchange trends. This model goes beyond basic price-tracking by incorporating correlated market features and technical indicators.

## Project Overview
This project develops a predictive pipeline for the **GBP/BDT** exchange rate. By leveraging **Long Short-Term Memory (LSTM)** neural networks, the model identifies complex temporal patterns in foreign exchange data to provide a 30-day recursive forecast.

### Key Features:
- **Multivariate Input:** Incorporates the **USD/BDT** rate as a leading indicator, recognizing the Taka's strong correlation with the US Dollar.
- **Feature Engineering:** Implements a **20-Day Moving Average (SMA)** to filter out daily market noise and highlight underlying trends.
- **Recursive Forecasting:** A custom loop that uses the model's own predictions as inputs to project a 30-day outlook.
- **Automated Pipeline:** Integrated with the `yfinance` API for real-time data ingestion.

## Tech Stack
- **Language:** Python 3.10+
- **Deep Learning:** TensorFlow / Keras
- **Data Analysis:** Pandas, NumPy
- **Scaling:** Scikit-Learn (MinMaxScaler)
- **Visualization:** Matplotlib

## Model Architecture & Results
The model consists of a stacked LSTM architecture with **Dropout layers (0.2)** to prevent overfitting. 

| Metric | Result |
| :--- | :--- |
| **Lookback Window** | 60 Days |
| **Optimizer** | Adam |
| **Loss Function** | Mean Squared Error (MSE) |
| **Final RMSE** | ~1.31 BDT |

### Sample Forecast
<img width="632" height="298" alt="image" src="https://github.com/user-attachments/assets/29b338cb-b5a6-4836-b65b-119e68efe00c" />

## How to Run
Clone the repository:
   ```bash
   git clone [https://github.com/your-username/Forex-Price-Prediction-LSTM.git](https://github.com/your-username/Forex-Price-Prediction-LSTM.git)
