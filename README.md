# Machine Learning Swing Trading Model

A quantitative trading research project that uses machine learning and technical market features to identify potential short-term swing trading opportunities in U.S. equities.

## Project Overview

The goal of this project is to build an end-to-end machine learning pipeline for analyzing historical stock-market data and estimating future short-term price movement.

Rather than relying on a single technical indicator, the model combines price trends, momentum, volatility, volume, and previous-session market behavior into a larger feature set used for machine-learning predictions.

The project was developed in Python using Google Colab.

## Data Pipeline

Historical market data is collected and transformed into model-ready features before training and evaluation.

The pipeline includes:

* Historical OHLCV market data
* Data cleaning and preprocessing
* Time-series feature engineering
* Target construction for future price movement
* Model training and prediction
* Model evaluation

## Feature Engineering

The model incorporates technical and market-behavior features including:

* Simple Moving Averages (SMA)
* Exponential Moving Averages (EMA)
* Relative Strength Index (RSI)
* Bollinger Bands
* VWAP
* Price and volume volatility
* Previous-day returns
* Previous-day trading range
* Previous-session volume
* After-hours market behavior
* Overnight price gaps
* Price relative to the previous regular-session close

## Machine Learning

The primary model used in this project is **XGBoost**.

The model is trained on engineered market features to learn relationships between recent market behavior and subsequent short-term price movement.

Because financial data is time-dependent, the project is designed around chronological market observations rather than treating the dataset as ordinary randomly ordered data.

## Technologies

* Python
* Pandas
* NumPy
* XGBoost
* scikit-learn
* Finnhub API
* Google Colab
* Git / GitHub

## Project Status

This project is an ongoing quantitative research project. Current work focuses on improving feature engineering, model evaluation, and testing the robustness of predictions across different stocks and market conditions.

## Disclaimer

This project is for educational and research purposes only. It is not intended to provide financial advice or live trading recommendations.
