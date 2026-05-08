# HASTS Projects (R2418461)

Welcome to my central repository for HASTS deliverables. This repository contains quantitative analysis and financial time series projects, including algorithms, error correction modeling, and statistical arbitrage analysis.

## 📁 Repository Contents

* **`HASTS 211/`**: Contains initial project files, coursework, and foundational data analysis.

---

## 🚀 Highlighted Work: Project 3 - Cointegration & ECM

### Overview
This project focuses on modeling non-stationarity and finding a long-term mathematical equilibrium between multiple financial assets. 

* **Topic:** Cointegration and Error Correction Models (ECM).
* **Data:** Daily closing prices of Apple Inc. (AAPL) and Microsoft Corp. (MSFT) from 2018 to 2025 (sourced via Yahoo Finance).
* **Objective:** To use the Engle-Granger two-step method to prove cointegration between AAPL and MSFT, calibrate the speed of adjustment ($\gamma$), and use these findings to formulate a market-neutral Statistical Arbitrage (Pairs Trading) strategy.

### Core Files
* `project3_cointegration.ipynb`: The executable Jupyter Notebook containing all Python code. It handles data fetching, OLS regressions, Augmented Dickey-Fuller (ADF) stationarity testing, and diagnostic chart generation.
* `project3_report.tex` / `.pdf`: The comprehensive academic report detailing the mathematical definitions, parameter interpretations, model damage assessment, and final investment deployment instructions.

### How to Run the Cointegration Model
1. Clone this repository or download the `.ipynb` file.
2. Open the notebook using a local Jupyter environment or upload it directly to [Google Colab](https://colab.research.google.com/).
3. Ensure the necessary dependencies are installed: 
   ```bash
   pip install yfinance pandas numpy statsmodels matplotlib
