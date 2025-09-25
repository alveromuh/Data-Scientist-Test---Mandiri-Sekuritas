# Data-Scientist-Test---Mandiri-Sekuritas
Welcome to Repository for Data Scientist Test at Mandiri Sekuritas. Presented by Muhammad Alvero Johansyah

This repository contains my solution for the Data Scientist Test at Mandiri Sekuritas.
The project focuses on forecasting stock's daily return using Long Short-Term Memory (LSTM) and Heuristic Stock Seelection Algorithm

Utilizing 225 Dataset incompanies that got in S&P500 in time range 2022-01-01 until 2024-12-31. Crawling data from yahoo finance to get historical financial features. Highlighting Performance of LSTM & Heuristic Stock Selection for Prediction %Recommendation in Daily Return target.

This project schema is clearly following to a paper "An Advisor Neural Network framework using LSTM-based Informative Stock Analysis" with Little modified in hyperparametertuning using Bayesian Optimization.

📂 Project Structure

LSTM_Stock_Forecasting_Alvero_DS.ipynb → Jupyter Notebook containing Data Ingestion, Forecasting Unit, Advice Stock Selection Unit, and Results & Visualization.

Approach: 

1. Data Ingestion
- Load and clean stock price dataset
- Feature engineering Seasonal Data & Technical Indicator
- News data is not used due to limited access
- Generate training and test splits
- Normalize features, one-hot encoding, etc

2. Forecasting Unit
- Build an LSTM-based neural network using TensorFlow/Keras
- Tune hyperparameters & find the best time window (sequence length, hidden units, dropout, optimizer)
- Use metrics such as RMSE/MSE/MAE for error evaluation
- Train and validate the model on technical and seasonal data

3. Advice Unit by Heuristic Stock Selection algorithm
- Give Best 5 Stocks based on output of LSTM in daily
- Use metrics such as RMSE/MSE/MAE for error evaluation
- Re rolling & Re train the data after forecasting in daily to give the best forecast in other day

4. Results & Visualization
- Knowing the performance by comparing the actual daily return
- Get to know portfolio performance return by simulating in test dataset on advice unit

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

All Data, Model, Code can also access & view on this Google Drive Link:
https://drive.google.com/drive/folders/1Uw_XOq1Pbjhxib_RtLQ5lFcOKTdKDtOL?usp=drive_link
