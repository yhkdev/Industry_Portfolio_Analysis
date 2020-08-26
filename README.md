# Fintech Project 1 - Industry & Economics Analysis

**Goal**: Find if there are correlation between industries and economic indicators

**Motivation**: To create a better portfolio out of the stocks I am invested in, or have invested in before

### Questions:

* What are the most uncorrelated industries?
* If there are correlation amongst industries, do these change over different time periods at all?

### Hypothesis: 


### Resources/Metrics Used
* **Industries**: Gaming, Oil, Defense, Big Tech, Finance, Airlines, Waste Service
* **Technology**: Python (Pandas, Seaborn, Requests, Json), Jupyter-lab
* **Data Source**: Alpha Vantage
* **Statistic Techniques**: corr, beta, std, ci, sharpe ratio

#### Industries:

* **Gaming** - EA, TTWO, ATVI
* **Oil** - XON, CVX
  * Upstream: COP, HAL
  * Mid/Downstream: KMI, PSX, EPD, ET, PAA, 
* **Defense** - LMT, RTN, LDOS, BA, NOC, GD, OSK, KBR
* **Big Tech** - FB, AAPL, AMZN, GOOG, MCST, IBM, INTC, CSCO, NVDA, MU, SQ, PYPL
* **Finance** - GS, JPM, MS, BAC, C, CS, UBS
* **Airlines** - UAL, LUV, DAL, AAL, ALK, JBLU, SAVE
* **Waste services** - WM, RSG, WCN


**Iterative Checkpoints**:

1. Gaming industry stock analysis
   a. Get EA, TTWO, ATVI
   b. Clean - date as index. col of tickers. rows of closing price per col.
   c. Stat Analysis - daily_return, cum_return, daily_std, annualized_std, annualized_sharpe, etc.
   
2. All portfolio stock analysis

   a. Get all other stocks for other industries listed above

   b. Group stocks into it's own industry portfolios

   b. Stat Analysis - Same as checkpoint 1, but for portfolios, not individual stocks

3. Select individual industries stock analysis

4. Relation - Between Industries

5. Relation - Between stocks in entire portfolio


#### Other considerations: Economics

Question
* Do gaming companies/stocks do well as unemployment rises?
* How correlated are common economic indicators with stock prices? 

Hypothesis
* Gaming industries do well as unemployment rises because more people play games
* Defense stocks are good hedge against economic downturns. They are necessary for the country so government will continue buying from them.
* Waste service stocks are uncorrelated with most other industry stocks and necessary regardless of economic downturn. Therefore, it is safer to invest in compared to other industries even in economic downturn. 

Resources/Metrics Used
* **Economics Indicators**: Unemployment, CPI, GDP, T-bond 10 yr yield, S&P 500
* **Data Source**: DBnomics