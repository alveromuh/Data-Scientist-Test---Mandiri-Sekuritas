# Data-Scientist-Test---Mandiri-Sekuritas
Welcome to Repository for Data Scientist Test at Mandiri Sekuritas. Presented by Muhammad Alvero Johansyah

This repository contains my solution for the Data Scientist Test at Mandiri Sekuritas.
The project focuses on forecasting stock prices using Long Short-Term Memory (LSTM)

Utilizing 225 Dataset in every companies that got in SNP500 in time range 2022-01-01 until 2024-12-31. Crawling data from yahoo finance to get historical financial features

📂 Project Structure

LSTM_Stock_Forecasting_Alvero_DS.ipynb → Jupyter Notebook containing data preprocessing, model training, evaluation, and visualization.

Approach: 

1. Data Preparation
- Load and clean stock price dataset
- Feature engineering Seasonal Data & Technical Indicator
- News data is not used due to limited access
- Generate training and test splits
- Normalize features, one-hot encoding, etc

2. Modeling
- Build an LSTM-based neural network using TensorFlow/Keras
- Tune hyperparameters (sequence length, hidden units, dropout, optimizer)
- Train and validate the model on historical price data

4. Evaluation
- Compare predicted vs actual prices
- Use metrics such as RMSE/MAE for error evaluation
- Plot stock price forecasts to visualize performance

Tech Stack:
- Python 3
- Jupyter Notebook
- TensorFlow / Keras
- NumPy, Pandas
- Matplotlib, Seaborn

Forecasting Unit & Advice Unit Stock Selection
1. in Forecasting unit, which used LSTM Architecture is in time range: 2022-02-22 until 2024-10-31. In this step i split the data based on train, validation, and test for finding the best performance purposes.
2. In Advice unit, which use 2024-11-01 until 2024-12-31. I use this timeframe for test set in advice unit. In this range, the puspose is to get best 5 stocks selection with heuristic stock selection after forecasting 200+ stocks in SNP500.

Results:
In test set on advice unit (Prediction set), The Portfolio get 54% return based on the performance of LSTM Forecasting and Heuristic Stock Selection Algorithm.

Visualizations show how predicted prices align with historical stock data.

(See notebook for detailed plots and results.)
