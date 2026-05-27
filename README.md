# HMM × Hurst Regime Detection Trading System

A quantitative finance and machine learning project focused on detecting hidden market regimes using **Hidden Markov Models (HMM)** and validating market behavior using the **Hurst Exponent**.

The goal of this project is to identify whether markets are:

* Trending
* Mean Reverting
* Random/Noisy

and use this information to build smarter, adaptive trading strategies.

---

## Project Motivation

Financial markets constantly shift between different regimes such as:

* High volatility
* Low volatility
* Bullish trends
* Bearish trends
* Sideways consolidation

Most traditional strategies fail because they assume market conditions remain constant.

This project attempts to solve that problem by combining:

* Probabilistic regime detection
* Statistical time-series analysis
* Quantitative trading concepts
* Machine learning techniques

---

# Core Concepts

## 1. Hidden Markov Model (HMM)

The Hidden Markov Model is used to detect hidden market states from observable financial data such as:

* Returns
* Volatility
* Momentum

The model probabilistically classifies the market into different regimes.

### Example Regimes

* Strong Bullish Trend
* Bearish Trend
* High Volatility State
* Mean-Reverting State

---

## 2. Hurst Exponent

The Hurst Exponent measures the persistence or memory of a time series.

### Interpretation

| Hurst Value | Market Behavior |
| ----------- | --------------- |
| H > 0.5     | Trending        |
| H < 0.5     | Mean Reverting  |
| H ≈ 0.5     | Random Walk     |

The Hurst Exponent acts as a confirmation layer for regime validation.

---

# Project Pipeline

```text
Data Collection
       ↓
Data Cleaning & Preprocessing
       ↓
Exploratory Data Analysis (EDA)
       ↓
Feature Engineering
       ↓
Hurst Exponent Calculation
       ↓
HMM Training
       ↓
Regime Detection
       ↓
Signal Generation
       ↓
Backtesting
       ↓
Performance Evaluation
```

---

# Features Used

The project uses several quantitative indicators and statistical features, including:

* Log Returns
* Rolling Volatility
* Moving Averages
* Momentum Indicators
* Hurst Exponent
* Regime Probabilities
* Hidden State Labels

---

# Technologies & Libraries

## Programming Language

* Python

## Libraries

* pandas
* numpy
* matplotlib
* seaborn
* scipy
* scikit-learn
* hmmlearn
* yfinance

---

# Exploratory Data Analysis (EDA)

EDA was performed to:

* Understand price behavior
* Analyze volatility clustering
* Identify return distributions
* Detect trends and anomalies
* Visualize regime shifts

Some visualizations include:

* Price charts
* Rolling volatility
* Return distributions
* Regime plots

---

# Model Workflow

## Step 1 — Data Collection

Historical market data is collected using Yahoo Finance APIs.

## Step 2 — Feature Engineering

Important statistical and technical features are generated.

## Step 3 — Hurst Calculation

The Hurst Exponent is calculated over rolling windows.

## Step 4 — HMM Training

The Hidden Markov Model is trained using engineered features.

## Step 5 — Regime Detection

The trained HMM identifies hidden market states.

## Step 6 — Validation

Detected regimes are validated using Hurst behavior and market characteristics.

## Step 7 — Backtesting

Strategy performance is tested across detected market regimes.

---

# Objectives

* Understand hidden market structure
* Detect regime changes dynamically
* Build adaptive trading systems
* Improve robustness of quantitative strategies
* Combine machine learning with financial statistics

---

# Future Improvements

* Live market regime detection
* Multi-asset support
* Deep learning integration
* Portfolio optimization
* Reinforcement learning based execution
* Automated trading deployment

---

# Results & Insights

The project demonstrates that:

* Market regimes can be probabilistically identified
* Hurst Exponent helps validate market persistence
* Different regimes exhibit different trading characteristics
* Adaptive systems can outperform static assumptions

---

# Folder Structure

```text
├── data/
├── notebooks/
├── models/
├── outputs/
├── plots/
├── README.md
└── requirements.txt
```

---

# Installation

```bash
git clone <your-repository-link>

cd hmm-hurst-regime-detection

pip install -r requirements.txt
```

---

# Running the Project

Open the Jupyter Notebook:

```bash
jupyter notebook
```

Run the notebook step-by-step to:

* Train the HMM
* Calculate Hurst values
* Detect market regimes
* Generate trading insights

---

# Disclaimer

This project is for educational and research purposes only.

It does not constitute financial advice or investment recommendations.

---

# Author

Priyal Jain

Interested in:

* Quantitative Finance
* Algorithmic Trading
* Machine Learning
* Statistical Modeling
* Market Microstructure
