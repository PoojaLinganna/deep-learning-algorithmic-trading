# Deep Learning for Finance – Algorithmic Trading

## Project Overview

This project implements a machine learning and deep learning framework for cryptocurrency trend prediction and quantitative trading strategy evaluation.

The objective is to predict next-day price direction and evaluate the financial performance of different models using risk-adjusted metrics.

---

## Dataset

- Cryptocurrency historical data (AAVE)
- Daily OHLCV data
- Market capitalization included
- Time-series sorted chronologically
- Train: 70% | Validation: 15% | Test: 15%

---

## Feature Engineering

The following financial and technical indicators were engineered:

- Daily Returns
- Spread (High − Low)
- Volume Change
- Moving Averages (MA5, MA10, MA21)
- Momentum (5, 10, 21 days)
- Rolling Volatility (10, 21 days)
- Market Capitalization

Target Variable:
- Binary classification of next-day return direction

---

## Models Implemented

### 1. Logistic Regression (Baseline Model)
- Linear classifier
- Benchmark for comparison

### 2. Multi-Layer Perceptron (MLP)
- Dense layers with Dropout
- Non-linear feature learning

### 3. LSTM (Long Short-Term Memory)
- Captures temporal dependencies
- Sequence-based modeling
- Early stopping for regularization

---

## Feature Selection

Random Forest feature importance was used to:
- Rank engineered features
- Select top predictors
- Reduce noise and overfitting risk

---

## Evaluation Metrics

### Classification Metrics
- Accuracy
- ROC-AUC
- Confusion Matrix
- Classification Report

### Financial Performance Metrics
- Sharpe Ratio (Risk-adjusted return)
- Maximum Drawdown (Risk exposure)
- Equity Curve comparison
- Buy & Hold benchmark

---

## Backtesting Framework

A custom backtesting engine was implemented with:

- Initial capital: $1,000,000
- Maximum position size: 50% of equity
- Whole-share constraint
- Trade log generation
- Daily P&L tracking
- Yield curve visualization

---

## Key Findings

- LSTM captures time-series structure better than static models.
- Deep learning improves directional prediction stability.
- Risk-adjusted returns outperform Buy & Hold under certain conditions.
- Volatility plays a significant role in short-term performance.

---

## Business Impact

- Supports systematic trading strategy design
- Enhances risk-adjusted portfolio performance
- Demonstrates application of deep learning in financial markets
- Bridges ML modeling with real financial evaluation

---

## Tech Stack

- Python
- NumPy
- Pandas
- Scikit-learn
- TensorFlow / Keras
- Matplotlib

---

## Future Improvements

- Hyperparameter optimization (Grid / Bayesian Search)
- Transaction cost modeling
- Slippage simulation
- Multi-asset portfolio extension
- Reinforcement Learning-based trading

---

## Author

Pooja L  
Master’s Student in Data Analytics  
Focused on Machine Learning & Quantitative Finance
