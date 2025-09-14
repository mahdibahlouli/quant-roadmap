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

- LeetCode: medium arrays/trees ([LeetCode Trees](https://leetcode.com/tag/tree/))
- pandas: datetime conversion, resample daily→weekly, rolling mean/volatility
- Mini-exercise: plot 20, 50, 200-day moving averages\
  **Resource:** [Statsmodels Time Series Examples](https://www.statsmodels.org/stable/examples/index.html)

**Day 6 – Mini-Project 1**

- QuickKit #1: Load 5 tickers, compute daily returns, moving averages, volatility
- Plot line charts & histograms
- Compute correlation matrix\
  **Resource:** [pandas plotting docs](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.plot.html) AND [Matplotlib Docs](https://matplotlib.org/stable/gallery/index.html)

**Day 7 – Review / Buffer**

- Review notebooks, repeat exercises if unclear
- Optional: watch 1 short pandas/NumPy video ([YouTube Pandas Tutorial](https://www.youtube.com/watch?v=vmEHCJofslg))
- Light LeetCode practice
- Plan Week 2

---

## Week 2: Probability, Stats, Time Series

**Day 8 – Probability Simulations**

- Simulate coin toss, dice, stock returns
- Compute mean, variance, histogram\
  **Resource:** [MIT OCW 18.05 Probability](https://ocw.mit.edu/courses/18-05-introduction-to-probability-and-statistics-spring-2014/) OR [Khan Academy Probability & Stats](https://www.khanacademy.org/math/statistics-probability)

**Day 9 – Hypothesis Testing**

- Notebook: t-test, z-test using `scipy.stats`
- Exercise: test if mean return of BTC = ETH\
  **Resource:** [SciPy Stats Docs](https://docs.scipy.org/doc/scipy/reference/stats.html) OR [StatQuest Hypothesis Testing](https://www.youtube.com/watch?v=0zZYBALbZgg)

**Day 10 – Rolling Statistics**

- Exercise: compute rolling mean/volatility for multiple tickers
- Plot series\
  **Resource:** [pandas Rolling Docs](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.rolling.html)

**Day 11 – Autocorrelation / Partial Autocorrelation**

- Compute ACF / PACF for 1 asset
- Plot results\
  **Resource:** [Statsmodels ACF/PACF](https://www.statsmodels.org/stable/generated/statsmodels.tsa.stattools.acf.html)

**Day 12 – Mini-Project 2**

- Probability & hypothesis testing notebook (2–3 tickers)
- Save results + short reflections\
  **Resource:** MIT OCW 18.05 AND Statsmodels examples

**Day 13 – Review / Buffer**

- Re-do unclear exercises, log takeaways
- Optional light LeetCode practice

**Day 14 – Light recap**

- Review Week 2 notebooks, add comments + observations
- Plan Week 3

---

## Week 3: Portfolio, CAPM, Backtesting

**Day 15 – Portfolio Basics**

- LeetCode: medium arrays ([LeetCode Medium Arrays](https://leetcode.com/tag/array/))
- Notebook: compute portfolio returns, weights, and expected return
- Exercise: calculate portfolio variance & standard deviation\
  **Resource:** [MIT 15.401 Finance Theory I](https://ocw.mit.edu/courses/15-401-finance-theory-i-fall-2008/) OR [NYU Courant Financial Engineering Lectures](https://www.youtube.com/playlist?list=PLq-Gm0yRYwTgJ0J9TrUW6S41sOMnpD6fr)

**Day 16 – Risk Metrics**

- Notebook: compute Sharpe ratio, max drawdown, rolling drawdown
- Mini-exercise: analyze 3-ticker portfolio\
  **Resource:** [QuantStart Risk Metrics](https://www.quantstart.com/articles/backtesting-systematic-trading-strategies-in-python-considerations-and-open-source-frameworks/) AND [Backtrader Docs](https://www.backtrader.com/docu/)

**Day 17 – CAPM & Beta**

- Notebook: compute beta, alpha, CAPM expected return
- Exercise: compare multiple assets
- Visualize risk vs return scatterplot\
  **Resource:** [Investopedia CAPM Guide](https://www.investopedia.com/terms/c/capm.asp) OR MIT 15.401

**Day 18 – Options Basics**

- Notebook: Black-Scholes pricing for call/put options
- Exercise: compute delta & gamma for 1 option\
  **Resource:** [QuantStart Black-Scholes](https://www.quantstart.com/articles/Black-Scholes-Made-Easy/) OR [Investopedia Options Basics](https://www.investopedia.com/options-basics-tutorial-4583012)

**Day 19 – Backtesting Strategy Basics**

- Notebook: moving average crossover strategy, compute returns
- Exercise: simulate simple buy/sell signals\
  **Resource:** [Backtrader Docs](https://www.backtrader.com/docu/) AND [QuantStart Backtesting](https://www.quantstart.com/articles/Event-Driven-Backtesting-with-Python-Part-I/)

**Day 20 – Mini-Project 3**

- Backtesting notebook: multiple assets, moving average + volatility strategy
- Plot equity curve & drawdown\
  **Resource:** Backtrader docs AND matplotlib

**Day 21 – Review / Buffer**

- Re-do unclear exercises, log takeaways, plan Week 4
- Optional light LeetCode practice

---
## 📅 Week 4: Machine Learning + Time Series (Super Detailed)

**Focus:** Apply statistical + machine learning methods to financial time series (ARIMA, GARCH, regression, PCA, forecasting).

---

**Day 22 – AR & MA Models (Time Series Foundations)**  
*File:* `notebooks/day22_ar_ma.ipynb`  

- **Topics:** Autoregressive (AR) & Moving Average (MA) models  
- **Steps:**  
  1. Import returns series.  
  2. Fit AR(1) model using `statsmodels.tsa.AR`.  
  3. Fit MA(1) model.  
  4. Plot predictions vs actual returns.  
  5. **Exercise:** Compare AR(1) vs MA(1) error.  

- **Resources:**  
  - [Statsmodels ARMA Tutorial](https://www.statsmodels.org/stable/examples/notebooks/generated/tsa_arma.html)  
  - [YouTube: AR vs MA vs ARMA Explained](https://www.youtube.com/watch?v=YxZzHkP4jXU)  

---

**Day 23 – ARIMA Forecasting**  
*File:* `notebooks/day23_arima_forecast.ipynb`  

- **Topics:** ARIMA (Autoregressive Integrated Moving Average).  
- **Steps:**  
  1. Fit ARIMA(1,1,1) on daily returns.  
  2. Forecast next 5 days.  
  3. Plot predicted vs actual returns.  
  4. **Exercise:** Compare ARIMA(1,1,1) vs AR(1).  

- **Resources:**  
  - [Statsmodels ARIMA Examples](https://www.statsmodels.org/stable/examples/notebooks/generated/tsa_arma_0.html)  
  - [YouTube: ARIMA Intuition](https://www.youtube.com/watch?v=YTe2e3R_GrY)  

---

**Day 24 – GARCH Volatility**  
*File:* `notebooks/day24_garch.ipynb`  

- **Topics:** GARCH (Generalized Autoregressive Conditional Heteroskedasticity) for volatility clustering.  
- **Steps:**  
  1. Use `arch` package to fit GARCH(1,1).  
  2. Compare predicted volatility vs rolling std.  
  3. Forecast next 5 days volatility.  
  4. **Exercise:** Apply to SPY & BTC.  

- **Resources:**  
  - [arch package tutorial](https://arch.readthedocs.io/en/latest/univariate/introduction.html)  
  - [YouTube: GARCH Explained Simply](https://www.youtube.com/watch?v=Og8zC4j8xhc)  

---

**Day 25 – ML Regression on Returns**  
*File:* `notebooks/day25_ml_regression.ipynb`  

- **Topics:** Machine learning regression with scikit-learn.  
- **Steps:**  
  1. Create lagged features: Return(t-1), Return(t-2), …  
  2. Train Linear Regression model.  
  3. Predict next-day return.  
  4. **Exercise:** Add Ridge regression and compare performance.  

- **Resources:**  
  - [Scikit-learn Linear Regression](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LinearRegression.html)  
  - [YouTube: Regression for Finance](https://www.youtube.com/watch?v=ZkjP5RJLQF4)  

---

**Day 26 – PCA / Factor Analysis**  
*File:* `notebooks/day26_pca.ipynb`  

- **Topics:** Principal Component Analysis (dimensionality reduction).  
- **Steps:**  
  1. Collect returns of 10 tickers.  
  2. Run PCA (`sklearn.decomposition.PCA`).  
  3. Identify 2–3 main factors.  
  4. Plot explained variance ratio.  
  5. **Exercise:** Interpret factors (e.g. “market factor”, “tech factor”).  

- **Resources:**  
  - [Scikit-learn PCA Docs](https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.PCA.html)  
  - [YouTube: PCA Intuition](https://www.youtube.com/watch?v=FgakZw6K1QQ)  

---

**Day 27 – Mini-Project 4 (Forecasting + Volatility)**  
*File:* `projects/mini_project4_forecasting.ipynb`  

- **Tasks:**  
  - Apply ARIMA, GARCH, Regression, PCA on the same dataset.  
  - Forecast next 5 days.  
  - Compare errors (RMSE).  
- **Deliverable:** Well-documented notebook with plots + reflections.  

---

**Day 28 – Review / Buffer**  
- Write `notes/week4.md`.  
- Re-do unclear steps.  
- Optional: Read academic paper on GARCH or PCA in finance.  

---

## 📅 Week 5: Rust + Crypto + Consolidation (Super Detailed)

**Focus:** Transition from quant finance to real-time trading systems and blockchain/DeFi.  

---

**Day 29 – Rust Order Book Simulator**  
*File:* `rust/orderbook/src/main.rs`  

- **Topics:** Order book basics.  
- **Steps:**  
  1. Define `Order { price, size, side }`.  
  2. Implement insert & remove.  
  3. Track bid-ask spread & mid-price.  
  4. **Exercise:** Add random order flow, plot mid-price.  

- **Resources:**  
  - [Rust Book](https://doc.rust-lang.org/book/)  
  - [YouTube: Rust for Beginners – freeCodeCamp](https://www.youtube.com/watch?v=MsocPEZBd-M)  

---

**Day 30 – Rust Async API**  
*File:* `rust/async_api/src/main.rs`  

- **Topics:** Async programming in Rust.  
- **Steps:**  
  1. Use `reqwest` to fetch dummy exchange API.  
  2. Parse JSON with `serde`.  
  3. Print top 5 assets by volume.  
  4. **Exercise:** Fetch Binance public data.  

- **Resources:**  
  - [Rust Async Book](https://rust-lang.github.io/async-book/)  
  - [Reqwest Docs](https://docs.rs/reqwest/)  

---

**Day 31 – Solana / Helius API**  
*File:* `notebooks/day31_helius_api.ipynb`  

- **Topics:** Fetch blockchain transaction data.  
- **Steps:**  
  1. Register free Helius API key.  
  2. Request token transfers.  
  3. Convert to pandas DataFrame.  
  4. Compute daily transaction counts.  
  5. **Exercise:** Plot transaction counts for 2 tokens.  

- **Resources:**  
  - [Helius API Docs](https://docs.helius.dev/)  
  - [Solana Docs](https://solana.com/docs)  

---

**Day 32 – Crypto Arbitrage Prototype**  
*File:* `notebooks/day32_arbitrage.ipynb`  

- **Topics:** Simple arbitrage strategy.  
- **Steps:**  
  1. Fetch prices from 2 exchanges.  
  2. Compute spread.  
  3. If spread > threshold → record trade.  
  4. **Exercise:** Simulate 1000 trades, compute P&L.  

- **Resources:**  
  - [Dune Analytics](https://dune.com/browse/dashboards)  
  - [CryptoQuant](https://cryptoquant.com/)  

---

**Day 33 – Mini-Project 5 (Rust + Python + Crypto)**  
*Files:*  
- Rust order book (`rust/orderbook/`)  
- Python notebook (`projects/mini_project5_crypto.ipynb`)  

- **Tasks:**  
  - Run Rust order book simulation.  
  - Fetch crypto data with Python.  
  - Combine signals into simple trading sim.  
- **Deliverable:** End-to-end pipeline across Rust + Python + Crypto.  

---

**Day 34 – Consolidation**  
- Merge all notebooks into clean folder structure.  
- Write summary notebook with highlights.  
- Add README with explanation for repo.  

---

**Day 35 – Final Review**  
- Write `notes/final_summary.md`.  
- Re-run all mini-projects.  
- Optional: prepare short presentation.  
