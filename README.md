# Maybank Stock Price Forecasting & GBM Modeling (STQA4113)

This repository contains the analysis and implementation for **STQA4113 Assignment (2025–26)**. The project focuses on statistical data analysis, stochastic modeling using **Geometric Brownian Motion (GBM)**, and predictive evaluation of Maybank's weekly stock price and trading volume.

---

## Project Overview & Objectives

As part of quantitative financial analysis, this project explores historical pricing data from **January 8th, 2023, to November 10th, 2025**, split into in-sample and out-sample periods to test forecasting accuracy. 

### Key Tasks Covered:
1. **Exploratory Data Analysis (EDA):** Computation of summary statistics (maximum, minimum, and standard deviation) for Maybank stock prices.
2. **Data Visualization:** Plotting price and volume against time, alongside rolling volatility ($\sigma$) and market drift ($\mu^M$).
3. **Stochastic Assumptions:** Outlining the theoretical assumptions underlying the Geometric Brownian Motion (GBM) model.
4. **Log Returns & Drift Calculation:** 
   - Weekly log returns computed using $ln(\frac{S_t}{S_{t-1}})$.
   - 1-year rolling average log return (raw drift, $\mu$) and standard deviation (volatility, $\sigma$).
   - Market drift derivation: $\mu^M = \mu - \frac{\sigma^2}{2}$.
5. **Out-of-Sample GBM Forecasting (Sep 15 – Nov 10, 2025):**
   - Forecasting prices using discretized GBM equations.
   - Constructing 5% / 90% confidence intervals and evaluating performance using **Mean Percentage Error (MPE)**.
6. **Dividend Incorporation:** 
   - Analyzing stock price dynamics post-dividend payout (average annual dividend of RM0.60/share).
   - Modifying the GBM formulation to account for dividends, re-forecasting, and comparing error metrics against the standard model.
7. **Critical Evaluation:** Assessing whether GBM is a suitable model for forecasting Maybank stock prices.

---
