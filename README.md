# 🏛️ PRINCE CHAUHAN — QUANTITATIVE RESEARCH & SYSTEMATIC DERIVATIVES

[![Build Status](https://github.com/pchauhanrajputpc-sketch/quant-research-portfolio/actions/workflows/tests.yml/badge.svg)](https://github.com/pchauhanrajputpc-sketch/quant-research-portfolio/actions)
[![Unit Tests](https://img.shields.io/badge/Unit%20Tests-29%2F29%20Passing-10B981.svg)](#)
[![SEBI Registered Research Analyst](https://img.shields.io/badge/SEBI%20Registration-Research%20Analyst-0284C7.svg)](https://www.sebi.gov.in/)
[![Experience](https://img.shields.io/badge/Experience-9%2B%20Years%20Quant%20Desk-193B56.svg)](#)
[![Primary Stack](https://img.shields.io/badge/Stack-Python%20%7C%20Polars%20%7C%20NumPy%20%7C%20SciPy-F59E0B.svg)](#)
[![Exchange Coverage](https://img.shields.io/badge/Markets-NSE%20%7C%20BSE%20Index%20%26%20Equities-10B981.svg)](#)
[![ATS CV](https://img.shields.io/badge/Curriculum%20Vitae-ATS%20Verified%20(1--Page)-EF4444.svg)](https://github.com/pchauhanrajputpc-sketch/quant-research-portfolio/tree/main/docs/PC_CV)

> 🔒 **INSTITUTIONAL COMPLIANCE & IP ISOLATION NOTICE**:  
> *All research models, volatility surfaces, backtesting engines, and risk gates in this public portfolio are self-contained educational implementations. Live order execution algorithms, high-frequency broker interfaces (DhanHQ), production alpha parameters, and real-money strategy books operate exclusively in a private, air-gapped trading desk environment.*

---

## 👨‍💻 Executive Profile

Senior Quantitative Analyst and Systematic Derivatives Strategist with **9+ years of experience** developing, validating, and deploying systematic options volatility, statistical arbitrage, and microstructure-aware execution architectures across Indian (NSE/BSE) index and single-stock derivatives.

- **Regulatory Status**: SEBI Registered Research Analyst • NISM Series-XV Certified
- **Education**: Bachelor of Commerce (Honours), Kirori Mal College, University of Delhi (1st Division) • CA Final G1 (ICAI, 78% Marks)
- **Primary Domain**: Volatility Surface Spline Modeling, Cross-Asset Cointegration, Market Regime Classification, Point-in-Time Vectorized Backtesting, and Asynchronous Execution Infrastructure.
- **Location**: New Delhi, India • Contact: `pchauhanrajput.pc@gmail.com`

---

## 🎯 7 Flagship Quantitative Research Showcases

Below are self-contained, reproducible quantitative research repositories demonstrating empirical rigor, no-lookahead safeguards, explicit transaction cost modeling, and statistical validation:

| # | Research Showcase | Quantitative Methodology | Institutional Alignment |
|---|---|---|---|
| **01** | **[Point-in-Time Backtesting Engine](https://github.com/pchauhanrajputpc-sketch/quant-research-portfolio/tree/main/research_showcases/point_in_time_backtester)** | Chronological event simulation, 0.50% turnover friction pre-deducted, exchange margin models (₹2.5L/₹1.8L/₹1.0L), 11-column canonical trade ledgers. | Rule L1–L22 Invariant Gate & WFO Validation |
| **02** | **[Options Volatility Surface & Greeks](https://github.com/pchauhanrajputpc-sketch/quant-research-portfolio/tree/main/research_showcases/options_volatility_surface)** | Black-Scholes inversion (Newton-Raphson/Brent), cubic spline & SVI surface fitting, arbitrage-free total variance constraints, dealer Gamma Exposure (GEX). | Real-time volatility skew & Greeks risk |
| **03** | **[Bank Nifty Basket Cointegration](https://github.com/pchauhanrajputpc-sketch/quant-research-portfolio/tree/main/research_showcases/banknifty_cointegration)** | Johansen rank cointegration test, dynamic rolling OLS hedge ratios, Ornstein-Uhlenbeck half-life estimation, mean-reverting spread Z-scores. | Statistical arbitrage across banking heavyweights |
| **04** | **[Market Regime & Volatility Gating](https://github.com/pchauhanrajputpc-sketch/quant-research-portfolio/tree/main/research_showcases/regime_allocation)** | Unsupervised K-Means clustering on Parkinson RV, IV/RV ratios, and return skewness. Counterfactual proof of reducing simulated portfolio max DD by 28%. | Dynamic gamma scaling & risk governance |
| **05** | **[Microstructure & Execution Simulator](https://github.com/pchauhanrajputpc-sketch/quant-research-portfolio/tree/main/research_showcases/execution_simulator)** | Order book queue priority, limit vs. market order fill probability, square-root market impact, and empirical proof of 1.8 bps market-crossing savings. | High-throughput async IPC & execution cost control |
| **06** | **[Institutional Tear Sheet Generator](https://github.com/pchauhanrajputpc-sketch/quant-research-portfolio/tree/main/research_showcases/institutional_tearsheet_generator)** | 6x2 KPI Scorecard, 8-year monthly returns heatmap grid, peak-to-trough underwater drawdown dynamics, publication-grade PDF report engine. | Executive CRO & Investment Committee reporting |
| **07** | **[Strategy Validator & Integrity Gate](https://github.com/pchauhanrajputpc-sketch/quant-research-portfolio/tree/main/research_showcases/strategy_validator_gate)** | 11-stage audit gate (Rules L1–L22), trade boundary clamping ($\le 15:14:59$), 2x friction stress testing, Monte Carlo drawdown cones (1,000 paths). | Systematic risk governance & anti-overfitting |

---

### ⚡ 10-Second Recruiter & Quant Quick-Start
To clone and execute all 29 research showcase test suites locally on any machine:
```bash
git clone https://github.com/pchauhanrajputpc-sketch/quant-research-portfolio.git
cd quant-research-portfolio
pip install numpy scipy polars reportlab
python -m unittest discover research_showcases
# Output: Ran 29 tests in 0.28s — OK
```

## 🔬 Quantitative Standards & Invariants

All research published in this portfolio strictly adheres to institutional risk governance:
1. **No-Lookahead Guarantee**: 100% causal point-in-time data handling. All indicator and signal logic references strictly historical bars ($t \le T-1$).
2. **Turnover Friction Reality**: Every backtest deducts 0.50% round-trip friction (brokerage, STT, exchange turnover fees, SEBI charges, GST, and 1-tick slippage buffer) before calculating returns.
3. **Regulatory Margin Conformance**: Sizing is strictly calibrated to Exchange Margin Benchmarks:
   - Short Straddles: ₹2,50,000 per lot
   - Naked Option Selling: ₹1,80,000 per lot
   - Hedged Option Spreads: ₹1,00,000 per lot
4. **Walk-Forward Overfitting Gate**: Models undergo 70% In-Sample training, 20% Out-of-Sample verification, and 10% Blind Holdout stress testing. Maximum allowable OOS Sharpe degradation is 30%.
5. **Sanitization**: All published code is 100% IP-sanitized for educational and technical demonstration purposes. Zero live broker credentials, active accounts, or proprietary firm data are included.

---

## 🛠️ Quantitative & Technical Stack

- **Quantitative Research**: Python 3.11+, Polars, DuckDB, NumPy, SciPy, Statsmodels, Scikit-Learn.
- **Financial Engineering**: Black-Scholes-Merton, SVI, Spline Smoothing, Greeks Sensitivity (Delta, Gamma, Vega, Theta, Rho), GEX, Cointegration (Johansen/ADF), Ornstein-Uhlenbeck.
- **Risk Governance & Attribution**: Parametric/Historical VaR, Conditional VaR (Expected Shortfall), Monte Carlo Stress Testing (1,000 paths), Sharpe/Sortino/Calmar, Maximum Drawdown Cones.
- **Systems Architecture**: Python Asyncio, Memory-Mapped IPC (`mmap`), WebSockets, SQLite, Flask, ReportLab PDF Engine, Python-Docx.
- **Testing & Quality Assurance**: PyTest, Python Unittest, Pre-flight AST Syntax Checking, Regression Smoke Gates.

---

## 📄 Official Documents & Verification

- 📄 **1-Page ATS Master CV (PDF)**: [`Prince Chauhan Quants Researcher CV - ATS Format.pdf`](https://github.com/pchauhanrajputpc-sketch/quant-research-portfolio/blob/main/docs/PC_CV/Prince%20Chauhan%20Quants%20Researcher%20CV%20-%20ATS%20Format.pdf)
- 📝 **Master Editable CV (DOCX)**: [`Prince Chauhan Quants Researcher CV - ATS Format.docx`](https://github.com/pchauhanrajputpc-sketch/quant-research-portfolio/blob/main/docs/PC_CV/Prince%20Chauhan%20Quants%20Researcher%20CV%20-%20ATS%20Format.docx)
- 💼 **LinkedIn Profile**: [linkedin.com/in/prince-chauhan-quant](https://www.linkedin.com/)
- 💻 **Public Quantitative Research Portfolio**: [github.com/pchauhanrajputpc-sketch/quant-research-portfolio](https://github.com/pchauhanrajputpc-sketch/quant-research-portfolio)

---
*Maintained by Prince Chauhan Quant Desk • New Delhi, India*
