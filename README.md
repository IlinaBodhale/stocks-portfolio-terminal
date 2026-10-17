# stocks-portfolio-terminal
# 📈 Live Robinhood API Portfolio Tracker & Risk Analytics Engine

A personal, production-ready "glass-box" asset management system built to track real capital deployments. This platform automates live market data pipelines via Python, logs secure API transactions, and replaces gamified fintech interfaces with deep, formula-driven risk analytics.

---

## 🎯 The Origin Story: Why I Built This

For my birthday, my parents gave me **\$1,000 of seed capital** to invest. When I logged into commercial brokerage apps, I noticed they felt more like video games than financial tools—obscuring the true mathematical risks behind a screen of bright buttons and push notifications. 

I didn't want to blindly click a button on a phone. I wanted full transparency over my data privacy and the math governing my portfolio. Using Python and **Claude Code** as my engineering pair, I built a local pipeline to securely pull my live trades and manage my own data lakes.

---

## 🛠️ Technical Stack & Frameworks

*   **System Orchestration:** Claude Code CLI (Iterative Prompt Engineering & Script Generation)
*   **Backend Automation Pipeline:** Python 3.x (`robin_stocks` API, `yfinance`, `pandas`, `openpyxl`)
*   **Analytics Engine & UI:** Formula-Driven Spreadsheet Architecture (Bloomberg Terminal-Style Theme)

---

## ⚡ Core Features & Live Implementation

### 1. Live Brokerage API Integration
*   **The Pipeline:** Integrated the `robin_stocks` Python library to securely authenticate and fetch chronological trade logs directly from my live Robinhood account.
*   **Security Protocol:** Formulated local security constraints utilizing system environment variables (`ROBINHOOD_USER`, `ROBINHOOD_PASS`) to ensure zero exposure of private API credentials or multi-factor authentication (MFA) keys on a public GitHub repository.

### 2. Automated Data Lakes
The Python automation script populates five distinct, isolated data tables within the local ecosystem:
*   `Trade_Log`: Complete transactional ledger synced straight from the brokerage API.
*   `Market_Data`: Time-series array tracking historical daily closing prices from Yahoo Finance.
*   `Reference_Data`: Categorical database housing sectors, industries, countries, and individual asset betas.
*   `Daily_Units` & `Daily_Cash`: Real-time tracking arrays computing automated share weights and remaining float balances.

### 3. Quantitative Risk Analytics
Instead of looking at flat numbers, I embedded macro-economic formulas directly into the spreadsheet cells so everything updates dynamically:
*   **Risk Metrics:** Value at Risk (95% & 99% VaR), CVaR, Sharpe Ratio, Sortino Ratio, and Maximum Drawdown.
*   **Correlation Matrix:** A dynamic, color-coded 3-scale conditional matrix showing cross-asset behavior.
*   **Macro Stress Testing:** Programmatic scenario simulation mapping portfolio elasticity during market crashes (-20%), corrections (-10%), or rapid rallies (+10%) adjusted for structural portfolio beta.

---

## 🚀 Execution & Daily Workflow

The repository utilizes a dedicated orchestration script that appends transactional data and live pricing metrics without rebuilding the core file structure.

### Execute Daily Fast-Sync (Fetch Live Prices)
```bash
python update_portfolio.py quick
```

### Manual Append & Brokerage Synchronization
```bash
python update_portfolio.py trade 34 2026-01-27 AAPL BUY 100 150.50
```

---

## 💡 System Design Reflections (AI as a Partner)

This project was built leveraging AI not as a shortcut, but as a compilation and debugging assistant. 

### My Major Engineering Breakthrough: Enforcing the "Glass-Box"
During initial script iterations, the AI kept trying to output flat, hardcoded numerical values into the Excel sheets. I had to systematically re-engineer my prompts to enforce a strict **Formula-Based Architecture**. 

Every calculation sheet now programmatically injects dynamic Excel syntax (like `=D2*F2`) instead of raw numbers. This means if I manually adjust a single price in the `Market_Data` tab, the entire analytics dashboard recalibrates instantly. I controlled the architecture; the AI just helped me execute it at a faster scale.
