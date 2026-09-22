# 🏛️ PRINCE CHAUHAN — QUANTITATIVE RESEARCH & SYSTEMATIC DERIVATIVES

[![Build Status](https://github.com/pchauhanrajputpc-sketch/quant-research-portfolio/actions/workflows/tests.yml/badge.svg)](https://github.com/pchauhanrajputpc-sketch/quant-research-portfolio/actions)
[![Unit Tests](https://img.shields.io/badge/Unit%20Tests-29%2F29%20Passing-10B981.svg)](#-10-second-recruiter--quant-quick-start)
[![SEBI Registered Research Analyst](https://img.shields.io/badge/SEBI%20Registration-Research%20Analyst-0284C7.svg)](https://www.sebi.gov.in/)
[![Experience](https://img.shields.io/badge/Experience-9%2B%20Years%20Quant%20Desk-193B56.svg)](#-executive-profile)
[![Primary Stack](https://img.shields.io/badge/Stack-Python%20%7C%20Polars%20%7C%20NumPy%20%7C%20SciPy-F59E0B.svg)](#%EF%B8%8F-quantitative--technical-stack)
[![Exchange Coverage](https://img.shields.io/badge/Markets-NSE%20%7C%20BSE%20Derivatives%20%26%20Equities-10B981.svg)](#-quantitative-standards--invariants)
[![ATS CV](https://img.shields.io/badge/Curriculum%20Vitae-ATS%20Verified%20(1--Page)-EF4444.svg)](https://github.com/pchauhanrajputpc-sketch/quant-research-portfolio/blob/main/docs/PC_CV/Prince%20Chauhan%20Quants%20Researcher%20CV%20-%20ATS%20Format.pdf)

> 🔒 **INSTITUTIONAL COMPLIANCE & IP ISOLATION NOTICE**:
> *All quantitative research models, volatility surfaces, backtesting engines, and risk gates in this public portfolio are self-contained educational implementations. Live order execution algorithms, high-frequency broker interfaces (DhanHQ), production alpha parameters, and real-money strategy books operate exclusively in a private, air-gapped trading desk environment.*

---

## 👨‍💻 Executive Profile

Senior Quantitative Analyst and Systematic Derivatives Strategist with **9+ years of experience** developing, validating, and deploying systematic options volatility, statistical arbitrage, and microstructure-aware execution architectures across Indian (NSE/BSE) index and single-stock derivatives.

- **Regulatory Standing**: SEBI Registered Research Analyst • NISM Series-XV Certified (Research Analyst)
- **Academic Foundation**: Bachelor of Commerce (Honours), Kirori Mal College, University of Delhi (1st Division) • CA Final G1 (ICAI, 78% Marks)
- **Core Competencies**: Volatility Surface Spline & SVI Modeling, Dealer Gamma Exposure (GEX), Point-in-Time Vectorized Backtesting, Cross-Asset Cointegration, Microstructure Execution Modeling, and Low-Latency Asynchronous Infrastructure.
- **Desk Location**: New Delhi, India • Contact: `pchauhanrajput.pc@gmail.com`

---

## 🎯 7 Flagship Quantitative Research Showcases

Below are 7 self-contained, fully reproducible quantitative research repositories demonstrating empirical rigor, causal no-lookahead data pipelines, explicit turnover cost deduction, and institutional risk governance:

| # | Research Showcase | Quantitative Methodology | Institutional Risk Governance |
|---|---|---|---|
| **01** | **[Point-in-Time Backtesting Engine](https://github.com/pchauhanrajputpc-sketch/quant-research-portfolio/tree/main/research_showcases/point_in_time_backtester)** | Chronological event simulation, dynamic clearing-house SPAN margin models, Bailey & Lopez de Prado Deflated Sharpe Ratio (DSR), and full-sample RMS Sortino semi-deviation. | 0.50% turnover friction pre-deducted, 11-column canonical trade ledgers, 100% point-in-time ticks. |
| **02** | **[Options Volatility Surface & Greeks](https://github.com/pchauhanrajputpc-sketch/quant-research-portfolio/tree/main/research_showcases/options_volatility_surface)** | Black-Scholes inversion (Newton-Raphson/Brent), natural cubic spline & SVI surface fitting, arbitrage-free total variance constraints, and aggregate dealer Gamma Exposure (GEX). | Monotonic variance bounds (total variance slope dw/dk >= 0), butterfly arbitrage filtering. |
| **03** | **[Bank Nifty Basket Cointegration](https://github.com/pchauhanrajputpc-sketch/quant-research-portfolio/tree/main/research_showcases/banknifty_cointegration)** | Johansen cointegration rank test, dynamic rolling OLS hedge ratios, Ornstein-Uhlenbeck spread half-life estimation, and mean-reverting Z-score execution. | Strict ADF stationarity verification (p-value < 0.05), bid-ask crossing and borrow drag pre-deducted. |
| **04** | **[Market Regime & Volatility Gating](https://github.com/pchauhanrajputpc-sketch/quant-research-portfolio/tree/main/research_showcases/regime_allocation)** | Unsupervised K-Means clustering on Parkinson High-Low Realized Volatility, IV/RV ratios, and return skewness. Dynamic short-gamma sizing reduction. | Empirical counterfactual proof of reducing simulated portfolio maximum drawdown by 28%. |
| **05** | **[Microstructure & Execution Simulator](https://github.com/pchauhanrajputpc-sketch/quant-research-portfolio/tree/main/research_showcases/execution_simulator)** | Order book queue priority, limit vs. market fill probability, square-root market impact (Impact proportional to Volatility * sqrt(Size / Volume)). | Quantitative attribution proving 1.8 bps market-crossing savings via asynchronous IPC and passive queues. |
| **06** | **[Institutional Tear Sheet Generator](https://github.com/pchauhanrajputpc-sketch/quant-research-portfolio/tree/main/research_showcases/institutional_tearsheet_generator)** | 6x2 KPI Scorecard, 8-year monthly returns heatmap grid, peak-to-trough underwater drawdown dynamics, and native Indian Rupee (₹) typography. | Publication-grade 3-page PDF report engine built with ReportLab for Executive CRO and Investment Committees. |
| **07** | **[Strategy Validator & Integrity Gate](https://github.com/pchauhanrajputpc-sketch/quant-research-portfolio/tree/main/research_showcases/strategy_validator_gate)** | 11-stage production audit gate (Rules L1–L22), intraday horizon boundaries (<= 15:14:59), 2x friction stress testing, and Monte Carlo drawdown cones (1,000 paths). | Systematic risk governance rejecting curve-fitted strategies, synthetic lookahead leaks, and negative carry wings. |

---

### ⚡ 10-Second Recruiter & Quant Quick-Start
To clone and execute all 29 research showcase test suites locally on any machine:
```bash
git clone https://github.com/pchauhanrajputpc-sketch/quant-research-portfolio.git
cd quant-research-portfolio
pip install numpy scipy polars reportlab
python -m unittest discover research_showcases
# Expected Output: Ran 29 tests in 0.28s — OK
```

---

## 🔬 Quantitative Standards & Invariants

All research published across this desk strictly adheres to institutional risk governance:
1. **No-Lookahead Guarantee**: 100% causal point-in-time data handling. All indicator and signal logic references strictly historical bars (t <= T-1). Zero future peeking.
2. **Turnover Friction & Cost Reality**: Every backtest deducts a baseline 0.50% round-trip execution cost (covering exchange STT, GST, SEBI turnover fees, stamp duty, bid-ask spread crossing, and market impact) before computing net returns.
3. **Dynamic Capital Allocation & Margin Constraints**: Position sizing is dynamically calibrated to clearing-house SPAN + Exposure margin benchmarks with explicit leverage caps and zero arbitrary cash haircuts (floor(Available Capital / Margin per Lot)).
4. **Walk-Forward Overfitting Gate**: Models undergo 70% In-Sample training, 20% Out-of-Sample verification, and 10% Blind Holdout stress testing. Maximum allowable Out-of-Sample Sharpe degradation is 30%.
5. **Parameter Plateau Mandate**: Optimal parameters must sit on a broad, stable performance plateau. Any parameter whose return collapses when shifted by +/-10% is classified as curve-fit noise and rejected.
6. **Sanitization**: All published code is 100% IP-sanitized for educational and technical demonstration purposes. Zero live broker credentials, active accounts, or proprietary trading desk parameters are included.

---

## 🛠️ Quantitative & Technical Stack

- **Quantitative Research**: Python 3.11+, Polars, DuckDB, NumPy, SciPy, Statsmodels, Scikit-Learn.
- **Financial Engineering**: Black-Scholes-Merton, SVI (Stochastic Volatility Inspired), Spline Smoothing, Greeks Sensitivity (Delta, Gamma, Vega, Theta, Rho), Dealer GEX, Cointegration (Johansen/ADF), Ornstein-Uhlenbeck Process.
- **Risk Governance & Attribution**: Parametric/Historical VaR, Conditional VaR (Expected Shortfall), Monte Carlo Stress Testing (1,000 paths), Bailey & Lopez de Prado Deflated Sharpe Ratio (DSR), Full-Sample RMS Sortino, Duration-Scaled Calmar, Maximum Drawdown Cones.
- **Systems Architecture**: Python Asyncio, Memory-Mapped IPC (`mmap`), High-Throughput WebSockets, SQLite, Flask, ReportLab PDF Engine.
- **Testing & Quality Assurance**: PyTest, Python Unittest, Pre-flight AST Syntax Checking, Regression Smoke Gates (112 atomic assertions).

---

## 📄 Official Documents & Verification

- 📄 **1-Page ATS Master CV (PDF)**: [`Prince Chauhan Quants Researcher CV - ATS Format.pdf`](https://github.com/pchauhanrajputpc-sketch/quant-research-portfolio/blob/main/docs/PC_CV/Prince%20Chauhan%20Quants%20Researcher%20CV%20-%20ATS%20Format.pdf)
- 💼 **Desk Inquiries & Collaboration**: [pchauhanrajput.pc@gmail.com](mailto:pchauhanrajput.pc@gmail.com) • [LinkedIn Network](https://www.linkedin.com/in/prince-chauhan-quant/)

---
*Maintained by Prince Chauhan Quant Desk • New Delhi, India*
