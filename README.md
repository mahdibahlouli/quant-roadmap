# QUANT ROADMAP

# Quant Roadmap — Super Detailed Daily Plan (5-Week Intensive, 8h/day)

This roadmap compresses the 16-week plan into 5 intensive weeks. Each day has **balanced, hands-on tasks** with coding, pandas/NumPy, probability/statistics, time series, quant finance, ML, backtesting, Rust/crypto, and mini-projects. **Resources are clearly marked as OR (pick one) or AND (use all).**

---

## Environment Setup (Before Day 1)

**Goal:** Reproducible Python + Rust environment.

**Steps:**

1. Create project directory: `quant-roadmap` with subfolders: `notebooks/`, `projects/`, `res/`, `notes/`
2. Python environment:

```bash
python3 -m venv venv
source venv/bin/activate  # Mac/Linux
pip install --upgrade pip
pip install pandas numpy scipy matplotlib statsmodels scikit-learn xgboost arch jupyterlab
```

3. Rust environment:

```bash
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
rustup update
cargo install cargo-edit
```

4. GitHub setup: initialize repo, commit README, add `.gitignore`
5. Notebook test: `jupyter lab`, load CSV, compute returns, plot line chart

**Deliverable:** working repo + `env_test.ipynb`

**Resources:**

* **Python & Jupyter**: official docs OR LinkedIn Learning “Learning Python”
* **Rust**: The Rust Programming Language book AND MIT 6.172 lectures

---

## Daily Schedule (8 hours/day)

| Time        | Task                                          |
| ----------- | --------------------------------------------- |
| 9:00–10:30  | LeetCode (arrays, hashmaps, DP, 1–2 problems) |
| 10:30–12:00 | Python/pandas/NumPy hands-on exercises        |
| 12:00–12:30 | Break                                         |
| 12:30–14:00 | Probability / Stats / Time Series exercises   |
| 14:00–15:00 | Lunch                                         |
| 15:00–16:30 | Quant Finance / Backtesting / ML exercises    |
| 16:30–18:00 | Mini-project / notebook consolidation         |
| 18:00–18:30 | Break                                         |
| 18:30–20:00 | Daily reflection, logging, saving notebook    |

---

## Week 1: Python + Pandas + NumPy + LeetCode

**Day 1 – Environment + Python Basics**

* LeetCode: easy array/string problems
* Notebook: variables, lists, dicts, functions
* Setup project folder + virtual environment, test CSV load
* Mini-exercise: compute daily returns for 1 stock
  **Resource:** pandas docs OR LinkedIn Learning module “Data Analysis with Python”

**Day 2 – pandas indexing & basic stats**

* LeetCode: easy/medium arrays
* Notebook: `loc`, `iloc`, slicing
* Exercise: compute mean, std, min, max returns for 3 tickers
* Visualize closing prices with matplotlib
  **Resource:** pandas docs OR LinkedIn Learning

**Day 3 – NumPy basics + vectorized calculations**

* LeetCode: hashmaps/arrays
* NumPy: array creation, slicing, basic ops
* Exercise: 20-day & 50-day rolling volatility
* Plot moving averages & volatility
  **Resource:** NumPy Quickstart OR LinkedIn Learning “Learning NumPy”

**Day 4 – pandas groupby + aggregation**

* LeetCode: stack/queue easy
* pandas: `groupby`, multi-index, pivot tables
* Exercise: compute monthly average returns, plot correlation heatmap
  **Resource:** pandas docs OR LinkedIn Learning

**Day 5 – Time Series Basics**

* LeetCode: medium arrays/trees
* pandas: datetime conversion, resample daily→weekly, rolling mean/volatility
* Mini-exercise: plot 20, 50, 200-day moving averages
  **Resource:** Statsmodels examples for time series

**Day 6 – Mini-Project 1**

* QuickKit #1: Load 5 tickers, compute daily returns, moving averages, volatility
* Plot line charts & histograms
* Compute correlation matrix
  **Resource:** pandas docs AND matplotlib documentation

**Day 7 – Review / Buffer**

* Review notebooks, repeat exercises if unclear
* Optional: watch 1 short pandas/NumPy video
* Light LeetCode practice
* Plan Week 2

---

## Week 2: Probability, Stats, Time Series

**Day 8 – Probability Simulations**

* Simulate coin toss, dice, stock returns
* Compute mean, variance, histogram
  **Resource:** MIT OCW 18.05 OR Khan Academy Statistics

**Day 9 – Hypothesis Testing**

* Notebook: t-test, z-test using `scipy.stats`
* Exercise: test if mean return of BTC = ETH
  **Resource:** SciPy docs OR online examples

**Day 10 – Rolling Statistics**

* Exercise: compute rolling mean/volatility for multiple tickers
* Plot series
  **Resource:** Statsmodels examples OR pandas docs

**Day 11 – Autocorrelation / Partial Autocorrelation**

* Compute ACF / PACF for 1 asset
* Plot results
  **Resource:** Statsmodels examples

**Day 12 – Mini-Project 2**

* Probability & hypothesis testing notebook (2–3 tickers)
* Save results + short reflections
  **Resource:** MIT OCW OR Khan Academy, Statsmodels examples

**Day 13 – Review / Buffer**

* Re-do unclear exercises, log takeaways
* Optional light LeetCode practice

**Day 14 – Light recap**

* Review Week 2 notebooks, add comments + observations
* Plan Week 3

---

## Week 3: Portfolio, CAPM, Backtesting

**Day 15 – Portfolio Basics**

* LeetCode: medium arrays
* Notebook: compute portfolio returns, weights, and expected return
* Exercise: calculate portfolio variance & standard deviation
  **Resource:** MIT 15.401 OR NYU Quant Lectures

**Day 16 – Risk Metrics**

* LeetCode: medium hashmaps
* Notebook: compute Sharpe ratio, max drawdown, rolling drawdown
* Mini-exercise: analyze 3-ticker portfolio
  **Resource:** QuantStart tutorials AND Backtrader docs

**Day 17 – CAPM & Beta**

* Notebook: compute beta, alpha, CAPM expected return
* Exercise: compare multiple assets
* Visualize risk vs return scatterplot
  **Resource:** MIT 15.401 OR NYU Quant Lectures

**Day 18 – Options Basics**

* Notebook: Black-Scholes pricing for call/put options
* Exercise: compute delta & gamma for 1 option
  **Resource:** QuantStart tutorials OR Investopedia Options Guide

**Day 19 – Backtesting Strategy Basics**

* Notebook: moving average crossover strategy, compute returns
* Exercise: simulate simple buy/sell signals
  **Resource:** Backtrader docs AND QuantStart tutorials

**Day 20 – Mini-Project 3**

* Backtesting notebook: multiple assets, moving average + volatility strategy
* Plot equity curve & drawdown
  **Resource:** Backtrader docs AND matplotlib

**Day 21 – Review / Buffer**

* Re-do unclear exercises, log takeaways, plan Week 4
* Optional light LeetCode practice

---

## Week 4: Machine Learning & Time Series Modeling

**Day 22 – AR & MA Models**

* Notebook: fit AR(1), MA(1) models on asset returns
* Plot predictions vs actual
  **Resource:** Statsmodels examples OR MIT 18.05 notes

**Day 23 – ARIMA Models**

* Notebook: ARIMA(1,0,1) forecasting for 1 asset
* Exercise: forecast next 5 days
  **Resource:** Statsmodels examples

**Day 24 – GARCH Volatility Modeling**

* Notebook: fit GARCH(1,1), compare with rolling volatility
* Exercise: 1–5 day volatility forecast
  **Resource:** `arch` package tutorial

**Day 25 – ML Regression on Returns**

* Notebook: linear regression using scikit-learn
* Exercise: predict returns from past 5-day returns
  **Resource:** MIT 6.036 OR Fast.ai course

**Day 26 – Factor Analysis / PCA**

* Notebook: compute PCA on returns to identify factors
* Exercise: explain 2–3 principal components
  **Resource:** Scikit-learn tutorials

**Day 27 – Mini-Project 4**

* Forecasting + volatility notebook for 1–3 assets, ARIMA + GARCH + regression
* Plot predictions, evaluate performance
  **Resource:** Statsmodels examples AND Scikit-learn tutorials

**Day 28 – Review / Buffer**

* Review Week 4 notebooks, reflections, plan Week 5
* Optional light LeetCode practice

---

## Week 5: Rust + Crypto / DeFi + Consolidation

**Day 29 – Rust Order Book Simulator**

* Notebook: basic Rust program to simulate limit order book
* Exercise: insert/remove orders, compute mid-price
  **Resource:** Rust book AND MIT 6.172 lectures

**Day 30 – Async API Connections**

* Notebook: Rust async API fetch from dummy exchange or Solana testnet
* Exercise: parse JSON, print top 5 assets by volume
  **Resource:** Rust async tutorials OR official Rust docs

**Day 31 – Solana / Helius Data Scraping**

* Notebook: fetch token transactions using Helius API
* Exercise: compute daily transaction count per token
  **Resource:** Solana Docs OR Helius API documentation

**Day 32 – Crypto Arbitrage Prototype**

* Notebook: simple arbitrage strategy between 2 tokens / DEXs
* Exercise: simulate profit/loss
  **Resource:** Dune Analytics OR CryptoQuant

**Day 33 – Mini-Project 5**

* Combine Rust + Python notebooks: simulate order book, fetch crypto data, compute signals
* Save project notebook with visualizations
  **Resource:** Rust book AND Backtrader docs

**Day 34 – Consolidation Day**

* Merge all notebooks (Weeks 1–5), clean code, add comments
* Create final GitHub repo structure
* Short reflection notes per week

**Day 35 – Review / Buffer / Light Practice**

* Re-do unclear exercises
* Optional: light LeetCode practice
* Prepare summary notebook for portfolio presentation

---

### ✅ Notes

* **OR** = pick one resource; **AND** = use all listed for that task
* Keep all exercises and mini-projects in notebooks
* Log daily progress (date, task, time spent, takeaway)
* Use breaks to avoid burnout
* End of each week: short reflection + plan next week
