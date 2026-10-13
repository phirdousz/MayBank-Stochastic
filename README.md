# Maybank Stock Price Forecasting & GBM Modeling (STQA4113)

This repository contains the group assignment analysis for **STQA4113 Stochastic Processes for Finance and Actuarial Science**. The project evaluates Maybank's weekly stock price and trading volume data from January 8, 2023, to November 10, 2025[cite: 1], applying **Geometric Brownian Motion (GBM)** to forecast out-of-sample prices and incorporating dividend adjustments.

---

## Executive Summary & Key Findings

1. **Exploratory Data Analysis:** Maybank exhibited a moderate price range (Maximum: RM10.80, Minimum: RM8.38) with a low standard deviation ($0.646$), reflecting its stability as a large-cap banking stock[cite: 5].
2. **GBM & Drift Dynamics:** Weekly log returns and 1-year rolling volatility ($\sigma$) were computed[cite: 6, 9]. The market drift ($\mu^M = \mu - \frac{\sigma^2}{2}$) showed a downward trend over time, indicating a slowing growth rate under volatility[cite: 12, 13].
3. **Out-of-Sample Forecasting:** Using in-sample data to forecast the period of September 15 to November 10, 2025, the standard GBM model kept actual market prices successfully within its 90% confidence interval, yielding a Mean Percentage Error (MPE) of approximately $0.00068$[cite: 14, 16, 17].
4. **Dividend Incorporation:** Factoring in Maybank’s average annual dividend of RM0.60 per share shifted the expected price path slightly downward, resulting in an MPE of approximately $0.00184$[cite: 18, 21]. While it increased short-term error marginally, it improved the theoretical realism of the model without altering return volatility[cite: 21, 22].
5. **Model Suitability:** GBM serves as a robust benchmark model for capturing long-term trends and risk bounds, but its assumption of constant drift and volatility limits its precision for short-term price reversals[cite: 22].

---

## Repository Structure

```text
├── data/
│   └── maybank_data.xlsx       # Weekly price and volume dataset
├── report/
│   └── assignment_report.pdf   # Full group assignment documentation
└── README.md                   # Project portfolio overview
