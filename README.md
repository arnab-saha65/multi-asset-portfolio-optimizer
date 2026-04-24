# Multi-Asset Portfolio Optimizer
### Wharton Business & Financial Modeling Capstone

![Excel](https://img.shields.io/badge/Tool-Microsoft%20Excel-217346?style=flat&logo=microsoft-excel)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)
![Course](https://img.shields.io/badge/Course-Wharton%20on%20Coursera-0056D2)

---

## Project Overview

Built a comprehensive multi-asset portfolio optimization 
model in Excel analyzing 10 US equities and market indices 
using 6 years of historical daily price data (2010–2016).
Applied Modern Portfolio Theory (Markowitz, 1952) to 
construct the efficient frontier and identify optimal 
portfolios under different constraints.

---

## Files

| File | Description |
|------|-------------|
| `portfolio_optimizer_wharton_project.xlsx` | Full Excel model |
| `Portfolio_Diversification_Presentation.pptx` | Project presentation |

---

## What Was Built

### Step 1 — Return Analysis
- Calculated daily returns for 10 stocks + DJI index
- Used Adjusted Close prices to account for dividends
  and stock splits
- 1,513 observations per security (Jun 2010 – Jun 2016)

### Step 2 — Summary Statistics
Computed for all 11 securities:
- Mean daily return
- Standard deviation
- Min / Max daily return
- Sharpe Ratio (risk-free rate = 0)

### Step 3 — Portfolio Optimization
**Two-Stock Portfolio (MSFT & WFC):**
- Efficient frontier construction (0% to 100% in 5% steps)
- Minimum Variance Portfolio via Excel Solver
- Tangent Portfolio (Maximum Sharpe Ratio)

**Ten-Stock Portfolio:**
- Full 10x10 covariance matrix
- Unconstrained optimization (short selling allowed)
- Long-only constrained optimization

### Step 4 — CAPM Analysis
- Regressed each stock's returns against DJI index
- Computed Alpha and Beta for all 10 securities
- Identified riskiest and least risky investments

### Step 5 — Mixed Asset Portfolio
- Optimized allocation between VBTLX (bonds) and
  VFIAX (equities) using Jan 2012 – Dec 2015 data
- Tested portfolio performance Jan – Jul 2016
- Compared against single stock AAPL

---

## Key Results

### Summary Statistics
| Stock | Mean Return | Std Dev | Sharpe |
|-------|------------|---------|--------|
| AAPL | 0.0839% | 1.651% | 0.051 |
| MSFT | 0.0746% | 1.481% | 0.050 |
| DIS | 0.0897% | 1.373% | 0.065 |
| TSLA | 0.2027% | 3.421% | 0.059 |
| DJI | 0.0443% | 0.911% | 0.049 |

### Two-Stock Optimization (MSFT & WFC)
| Portfolio | MSFT | WFC | Sharpe |
|-----------|------|-----|--------|
| Min Variance | 55.3% | 44.7% | 0.053 |
| Tangent | 68.1% | 31.9% | 0.053 |

### Ten-Stock Optimization
| Constraint | Sharpe | Key Holdings |
|------------|--------|--------------|
| Long-Only | 0.084 | DIS 38.8%, AAPL 17.1% |
| Short Selling | 0.088 | DIS 49.7%, AAPL 20.7% |

### CAPM Results
| Stock | Beta | Risk Level |
|-------|------|------------|
| TTM | 1.493 | 🔴 Highest |
| BIDU | 1.312 | 🔴 High |
| TSLA | 1.239 | 🔴 High |
| AAPL | 0.900 | 🟢 Lowest |

### Mixed Asset Portfolio (Step 5)
- Optimal weights: VBTLX 67.8% | VFIAX 32.2%
- Portfolio Sharpe: 0.4746
- Jan–Jul 2016: Portfolio +6.77% vs AAPL +7.94%
- Portfolio showed significantly lower volatility

---

## Key Findings

1. **Diversification reduces risk** — minimum variance
   portfolio (1.31% StdDev) is far below any individual stock
2. **Short selling unlocks alpha** — unconstrained Sharpe
   (0.088) beats long-only (0.084)
3. **Stability over volatility** — mixed portfolio never
   dropped below -0.62%/month vs AAPL's -10% in Jan 2016
4. **TTM is riskiest** (Beta 1.49), AAPL is least risky
   (Beta 0.90) among the 10 securities

---

## Tools Used

- Microsoft Excel (Solver, Data Analysis ToolPak)
- Mean-Variance Optimization (Markowitz)
- CAPM Regression Analysis
- Covariance Matrix Construction

---

## Course

**Wharton Business & Financial Modeling Specialization**
Coursera — Capstone Project
University of Pennsylvania, Wharton School

---

*Arnab Saha | April 2026*
