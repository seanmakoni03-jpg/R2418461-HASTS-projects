# Quantitative Finance & Time Series Analysis Portfolio

This repository contains two major research projects focusing on volatility modeling for derivatives trading and the implementation of equilibrium-based statistical arbitrage strategies.

## Portfolio Overview
---
### [Assignment 1] Derivatives Desk Volatility Modeling: Best-Practices & Infrastructure Handbook
**Focus:** Risk Management, Model Governance, and Infrastructure.

This document serves as an internal handbook for a quantitative research group at a derivatives desk. It bridges the gap between high-level executive strategy and deep-learning/statistical technicalities.

* **Executive Summary:** A strategic memo to the Head of Derivatives Trading detailing volatility audit results.
* **Infrastructure:** Analysis of data pipelines and computational requirements for real-time volatility estimation.
* **Technical Challenges:** In-depth discussion on over-parameterization, data noise, and non-stationarity.
* **Proposed Resolutions:** Implementation of LASSO regularization, Akaike Information Criterion (AIC) for model selection, and k-fold cross-validation to ensure out-of-sample robustness.
---
### [Assignment 2] Project 3: Modeling Non-Stationarity and Finding an Equilibrium
**Focus:** Cointegration, Error Correction Models (ECM), and Pairs Trading.

This assignment implements an end-to-end quantitative trading strategy using the Engle-Granger Two-Step method to model the relationship between Apple Inc. (AAPL) and Microsoft Corp. (MSFT).

* **Theory:** Definition and implementation of cointegration ($I(1)$ series forming an $I(0)$ spread).
* **Calibration:**
    * **Long-Run Equilibrium:** $log(AAPL_t) = -1.2308 + 1.0990 \\cdot log(MSFT_t)$.
    * **Speed of Adjustment ($\\gamma$):** Calibrated at **-0.0107** (p-value 0.002), indicating that 1.07% of the equilibrium error is corrected daily.
* **Statistical Arbitrage:** A deployment-ready framework using Z-score standardization of the spread to trigger mean-reversion trades.

---

## Technical Stack

The projects are implemented in Python using the following specialized libraries:

* **`yfinance`**: For automated retrieval of historical financial market data.
* **`statsmodels`**: Used for OLS Regression, Augmented Dickey-Fuller (ADF) stationarity testing, and ECM calibration.
* **`pandas` & `numpy`**: For time series manipulation, log transformations, and vectorized financial calculations.
* **`matplotlib`**: For generating diagnostic plots, price series visualizations, and spread analysis.

---

## Author

**Tashinga Sean Makoni** Student ID: R2418461  
Program: HDSC (Data Science and Systems)

---

## Bibliography

The theoretical foundations for these projects are based on the following authoritative sources:
1.  **Engle, R. F., & Granger, C. W. J.** (1987). Co-Integration and Error Correction: Representation, Estimation, and Testing.
2.  **Brooks, C.** (2019). *Introductory Econometrics for Finance*. Cambridge University Press.
3.  **Hull, J. C.** (2022). *Options, Futures, and Other Derivatives*. Pearson.
4.  **Tsay, R. S.** (2010). *Analysis of Financial Time Series*. Wiley.
---
