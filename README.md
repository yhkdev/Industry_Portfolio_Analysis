# Fintech Project 1

Industry & Economics Analysis

Goal: Find if there are correlation between industries and economic indicators

Motivation: To create a better portfolio out of the stocks I are invested in / have invested in before

Questions:
* What are the most uncorrelated industries?
* If there are correlation amongst industries, do these change over different time periods at all?
* Do gaming companies/stocks do well as unemployment rises?

Hypothesis: 
* Gaming industries do well as unemployment rises because more people play games
* Defense stocks are good hedge against economic downturns. They are necessary for the country so government will continue buying from them.
* Waste service stocks are uncorrelated with most other industry stocks and necessary regardless of economic downturn. Therefore, it is safer to invest in compared to other industries even in economic downturn. 

### Resources/Metrics Used
**Industries**: Gaming, Oil, Defense, Big Tech, Finance, Airlines, Waste Service
**Economics Indicators**: Unemployment, CPI, GDP, T-bond 10 yr yield, S&P 500
**Tech Packages**: Pandas, 
**Data Source**: Alpha Vantage, DBnomics
**Statistic Techniques**: corr, beta, std, ci, sharpe ratio

**Industries**:

* **Gaming** - EA, TTWO, ATVI
* **Oil** - XON, CVX
  * Upstream: COP, HAL
  * Mid/Downstream: KMI, PSX, EPD, ET, PAA, 
* **Defense** - LMT, RTN, LDOS, BA, NOC, GD, OSK, KBR
* **Big Tech** - FB, AAPL, AMZN, GOOG, MCST, IBM, INTC, CSCO, NVDA, MU, SQ, PYPL
* **Finance** - GS. JPM, MS, BAC, C, CS, UBS
* **Airlines** - UAL, LUV, DAL, AAL, ALK, JBLU, SAVE
* **Waste services** - WM, RSG, WCN


**Iterative Checkpoints**:

1. Gaming industry stock analysis
   a. Get EA, TTWO, ATVI
   b. Clean - date as index. col of tickers. rows of closing price per col.
   c. Stat Analysis - daily_return, cum_return, daily_std, annualized_std, annualized_sharpe, etc.
2. Relation -  Gaming industry & Unemployment
3. Relation - Gaming industry & Economics
4. Select industries stock analysis
5. Relation - Select industries & Economics
6. Relation - Between Industries