# GoldPriceLSTM
This notebook builds a time series model to predict gold prices using five years of historical data, aiding traders in forecasting future trends.

# XAUUSD LSTM Model for Gold Price Prediction

This repository contains the code for training and deploying a Long Short-Term Memory (LSTM) model with an attention mechanism to predict gold prices (XAUUSD). The model is trained on historical gold futures data and can be deployed as a Streamlit application to provide live trading suggestions.

## Overview

**Colab (Training & Backtesting):** This section focuses on data acquisition, preprocessing, model training, and backtesting.

## Colab Notebook

### Workflow

1.  **Data Import:** Fetches historical gold futures data using the `yfinance` library.
2.  **Feature Engineering:** Includes creating features, such as scaling the data with MinMaxScaler.
3.  **Model Building:** Constructs an LSTM model with multiple layers and dropout for regularization.
4.  **Model Training:** Trains the model on historical data, with the last year used as the test set.
5.  **Model Evaluation:** Evaluates the model's performance on the test set using metrics like Mean Absolute Percentage Error (MAPE).
6.  **Backtesting:** Visualizes model predictions against actual gold prices on the test set.
7.  **Model Saving:** Saves the trained model as `best_model.h5`.

### Libraries Used

*   `requests`: For making HTTP requests.
*   `pandas`: For data manipulation and analysis.
*   `numpy`: For numerical operations.
*   `matplotlib`: For basic data visualization.
*   `scikit-learn`: For data preprocessing (MinMaxScaler) and evaluation (MAPE).
*   `tensorflow`: For building and training the LSTM model.
*   `seaborn`: For enhanced data visualization.
*   `ta`: For technical analysis indicators.
*   `yfinance`: For fetching financial data.
*   `plotly`: For interactive plots.

### Setup and Installation

1.  **Install Dependencies:**
