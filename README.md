# Equity Research & Portfolio Optimization Study

> A multi-part quantitative finance project combining fundamental analysis of a listed Indian company with portfolio construction, optimization, and 3-year performance evaluation against the Nifty benchmark.

---

## Overview

This project performs a **two-pronged analysis** — first a deep-dive fundamental study of a mid-cap NSE-listed company, followed by construction and evaluation of a **5-stock diversified portfolio**. The portfolio is benchmarked against Nifty/Sensex over 3 years, and further optimized to construct both a **minimum variance portfolio** and a **Sharpe ratio-maximizing portfolio**.

Built as part of the Security Analysis and Portfolio Management course (**ECON F412 / FIN F313**) at **BITS Pilani, Pilani Campus**.

---

## Tools Used

| Tool | Purpose |
|---|---|
| Microsoft Excel | All analysis, modeling, and portfolio construction |
| NSE / BSE | Historical price data and financial statements |
| Screener.in / Trendlyne | Fundamental ratios and industry benchmarks |
| Moneycontrol | Dividend history, corporate actions |

---

## Project Structure

```
sapm-portfolio-study/
│
├── data/
│   └── stock_prices.xlsx            # Historical weekly price data for all 5 stocks + Nifty
│
├── SAPM_Assignment.xlsx             # Master Excel file with all analysis sheets
│   ├── Sheet 1 — Contributors
│   ├── Sheet 2 — Fundamental Analysis (FY23 & FY24)
│   ├── Sheet 3 — Price Movement Analysis
│   ├── Sheet 4 — Portfolio Construction & Returns
│   ├── Sheet 5 — Portfolio Evaluation (Sharpe, Treynor)
│   ├── Sheet 6 — Individual vs Portfolio Risk-Return
│   ├── Sheet 7 — Correlation Matrix
│   └── Sheet 8 — Optimized Portfolios (Min Variance & Max Sharpe)
│
└── README.md
```


*(Full table in `SAPM_Assignment.xlsx` Sheet 2)*

**DuPont ROE Breakdown:**
```
ROE = Net Profit Margin × Asset Turnover × Equity Multiplier
```

---

### Part II — Price Movement Analysis

| Metric | Value |
|---|---|
| Lifetime High | ₹ — |
| Lifetime Low | ₹ — |
| Current Price % discount to Lifetime High | —% |
| 52-week Avg Daily Volume | — shares |
| Dividend Type & History (past 2 years) | — |
| Stock Splits (past 2 years) | — |
| Share Buybacks (past 2 years) | — |
| Major M&A / Corporate Actions | — |

**Earnings Announcement Market Reaction (Past 4 Quarters):**

| Quarter | EPS Actual | EPS Estimate | Price Reaction |
|---|---|---|---|
| Q1 FY25 | — | — | —% |
| Q2 FY25 | — | — | —% |
| Q3 FY25 | — | — | —% |
| Q4 FY24 | — | — | —% |

---

### Part III — Portfolio Construction & Analysis

#### Portfolio Setup

- **Construction Date:** 1st April 2022
- **Primary Company Weight:** 30%
- **Remaining 4 stocks:** Value-weighted, selected from different sectors with MCAP ≥ ₹5,000 Cr
- **No rebalancing** post construction

| Stock | Sector | Weight |
|---|---|---|
| Primary Company | — | 30% |
| Stock 2 | — | —% |
| Stock 3 | — | —% |
| Stock 4 | — | —% |
| Stock 5 | — | —% |

---

#### a. Portfolio Performance vs Benchmark

Evaluated using weekly returns over 3 years (Apr 2022 – Mar 2025):

| Metric | Portfolio | Nifty/Sensex |
|---|---|---|
| 3-Year Return | —% | —% |
| Annualized Return | —% | —% |
| Standard Deviation | — | — |
| Sharpe Ratio | — | — |
| Treynor Ratio | — | — |
| Beta | — | 1.0 |

**Year-by-Year Performance Breakdown:**

| Year | Portfolio Return | Nifty Return |
|---|---|---|
| FY23 (Apr 22 – Mar 23) | —% | —% |
| FY24 (Apr 23 – Mar 24) | —% | —% |
| FY25 (Apr 24 – Mar 25) | —% | —% |

---

#### b. Individual Stock vs Portfolio: Risk-Return Analysis

Does diversification add value? Compared primary stock standalone vs full portfolio:

| Metric | Primary Stock | Portfolio |
|---|---|---|
| Annualized Return | —% | —% |
| Standard Deviation | — | — |
| Sharpe Ratio | — | — |
| Beta | — | — |

**Finding:** *(Fill in — e.g., "The portfolio offered lower volatility with comparable returns, confirming diversification benefits...")*

---

#### c. Optimized Portfolios

**Correlation Matrix (All 5 Stocks):**

| | Stock 1 | Stock 2 | Stock 3 | Stock 4 | Stock 5 |
|---|---|---|---|---|---|
| Stock 1 | 1.00 | — | — | — | — |
| Stock 2 | — | 1.00 | — | — | — |
| Stock 3 | — | — | 1.00 | — | — |
| Stock 4 | — | — | — | 1.00 | — |
| Stock 5 | — | — | — | — | 1.00 |

Using the correlation matrix, two optimized portfolios were constructed using **Solver in Excel**:

**i. Minimum Variance Portfolio**
- Objective: Minimize portfolio standard deviation
- Constraints: Weights sum to 1, no short selling

| Stock | Optimal Weight |
|---|---|
| Stock 1 | —% |
| Stock 2 | —% |
| Stock 3 | —% |
| Stock 4 | —% |
| Stock 5 | —% |
| **Portfolio Std Dev** | — |

**ii. Maximum Sharpe Ratio Portfolio (Nifty-mimicking)**
- Objective: Maximize Sharpe ratio to match/exceed Nifty's risk-adjusted return

| Stock | Optimal Weight |
|---|---|
| Stock 1 | —% |
| Stock 2 | —% |
| Stock 3 | —% |
| Stock 4 | —% |
| Stock 5 | —% |
| **Portfolio Sharpe** | — |

*(Full Solver setup and workings in `SAPM_Assignment.xlsx` Sheet 8)*

---

## Key Findings

Based on the data, the Portfolio is the clear winner. It generated a solid profit of  15.48%, whereas holding the individual stock (Bata) resulted in a significant  15.18% loss.

Strictly speaking, Bata had lower risk statistics (Standard Deviation of 0.22 vs 0.34 and Beta of 0.74 vs 1.10), meaning it was less volatile. However, low risk is useless if it leads to negative returns.

The Portfolio demonstrates a superior risk-reward pattern. The positive Coefficient of Variation (2.18) proves that the portfolio's higher volatility was justified because it delivered returns. Bata's negative metrics indicate a "dead loss" scenario where risk was taken for no reward.

Diversification proved highly beneficial. While it did not reduce volatility in this specific case, it saved the investor from Bata's specific failure. By spreading capital, the portfolio offset Bata's losses with gains from other assets, securing a positive outcome.

## How to Use

1. Clone or download the repository
2. Open `SAPM_Assignment.xlsx` in Microsoft Excel
3. Navigate sheets in order — all formulas and Solver configurations are preserved
4. To re-run Solver optimizations: Data → Solver → Solve (ensure Solver add-in is enabled)

---

## References

- Sharpe, W. F. (1966). *Mutual Fund Performance*
- Treynor, J. L. (1965). *How to Rate Management of Investment Funds*
- Bodie, Kane & Marcus — *Investments*
- NSE India Historical Data — [nseindia.com](https://www.nseindia.com)
- Screener.in — [screener.in](https://www.screener.in)

---

## Author

**Shivam Singla**
B.E. Computer Science Engineering, BITS Pilani (2027)
📧 F20230576@pilani.bits-pilani.ac.in
🔗 [LinkedIn](https://www.linkedin.com/in/shivam-singla-043ab53a8/) · [GitHub](https://github.com/shivam-bppc)

---

> *Built for academic purposes as part of ECON F412 / FIN F313 coursework at BITS Pilani. Not financial advice.*
