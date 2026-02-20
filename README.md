# Financial Data Analysis – MATLAB

Statistical analysis of a 5-stock portfolio using MATLAB, covering descriptive statistics, correlation analysis, moving averages, and regression modeling.

## Overview

Completed as part of **FINA 6332: Financial Mathematics** at Northeastern University (Fall 2025). The project analyzes daily log returns for five stocks across four analytical areas using MATLAB.

## Assets Analyzed

| Ticker | Company | Sector |
|--------|---------|--------|
| PFE | Pfizer | Healthcare |
| PG | Procter & Gamble | Consumer Staples |
| AVGO | Broadcom | Technology |
| MSFT | Microsoft | Technology |
| TSLA | Tesla | Consumer Cyclical |

## Analysis Summary

### Part 1: Descriptive Statistics
- Calculated daily/annualized mean returns, standard deviation, skewness, excess kurtosis, and Sharpe ratios
- AVGO delivered the strongest risk-adjusted performance (Sharpe: 0.95), while PFE and MSFT posted negative returns

### Part 2: Correlation & Covariance
- Built correlation and variance-covariance matrices with heatmap visualizations
- Mean portfolio correlation of 0.16 indicates strong diversification potential
- MSFT showed near-zero correlation with all other assets, making it an effective portfolio stabilizer

### Part 3: Moving Average Analysis
- Plotted daily log returns with 20-day moving averages for PFE and an equally weighted portfolio
- Equally weighted portfolio demonstrated smoother returns than individual stocks, confirming diversification benefits

### Part 4: Regression Analysis
- **Single regression:** Regressed returns on log volume for PFE and AVGO
- **Multiple regression:** Added high-low price range as a second predictor
- Both models showed R² < 1%, consistent with efficient market hypothesis — volume and price range have minimal predictive power for returns

## Key Findings

| Metric | PFE | PG | AVGO | MSFT | TSLA |
|--------|-----|-----|------|------|------|
| Annualized Return | -6.7% | 6.1% | 39.6% | -3.5% | 53.5% |
| Annualized Volatility | 27.6% | 21.0% | 41.7% | 16.4% | 67.0% |
| Sharpe Ratio | -0.24 | 0.29 | 0.95 | -0.21 | 0.80 |

## Tools Used

- MATLAB (descriptive statistics, regression, visualization)
- Microsoft Excel (data source)

## Files

- `MINIPROJECTTEAM06.mlx` — MATLAB Live Script with full analysis and visualizations
- `Fin_Math.xlsx` — Source data with daily prices and volumes for all five stocks
- `Mini_Project_Report.pdf` — Full written report with commentary and charts
