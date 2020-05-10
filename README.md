# Stocks-Data-Analysis

Project Background-

A stock (also known as equity) is a security that represents the ownership of a fraction of a corporation. This entitles the owner of the stock to a proportion of the corporation's assets and profits equal to how much stock they own. Numerous studies have shown that, over long periods of time, stocks generate investment returns that are superior to those from every other asset class. Whether we are considering buying or selling it, the decision can be aided by studying it. The historical data can help us judge the next likely move that the stock might make and the moves that are less likely. Traders looking to back-test a model or strategy can use simulated prices to validate its effectiveness. Excel can help with the back-testing using a monte carlo simulation to generate random price movements. 
If a company decreases or increases 1 per cent or 2 per cent, it could be due to a movement relative to the flow of the markets, it could be due to a large seller that just needed liquidity or there could have just been some counterparties that were slightly more eager to sell than the buyers. Public perception and human emotion are enough to move a stock by small amounts day in and day out.
The purpose of this study is to look at the stock movement, predict its prices and to realize the annual returns. 

Data-

The data was downloaded from Kaggle – S&P 500 stock data. It is a stock market index that measures the stock performance of 500 large companies listed on stock exchanges in the United States. It is one of the most followed equity indices, and many consider it to be one of the best representations of the U.S. stock market. Although the index includes only companies listed in the United States, companies not originating from the United States might be included in the future. It already includes many multi-national companies; companies in the index derive on average only 71% of their revenue in the United States. 
The Kaggle dataset has close to 650K rows of daily traded stocks between 2013 and 2018. For my analysis I have only considered Ebay’s stock for 2017 due to limitation with my system’s resources. Below link was used to download the same: -

https://www.kaggle.com/camnugent/sandp500

It contains the following variables – 
•	Date - in format: yy-mm-dd
•	Open - price of the stock at market open 
•	High - Highest price reached in the day
•	Low – Lowest price reached in the day
•	Close - Lowest price reached in the day
•	Volume - Number of shares traded
•	Name - the stock's ticker name
 

Simulation Models - 

The Monte Carlo method is a stochastic method to solve a statistical problem, and a simulation is a virtual representation of a problem. A Monte Carlo simulation considers a wide range of possibilities and helps reduce uncertainty. It is very flexible, allows us to vary risk assumptions under all parameters and thus model a range of possible outcomes. One can compare multiple future outcomes and customize the model to various assets and portfolios under review. 
Stocks are very prone to fluctuate after each trading day. To harness that random process a little better, Monte Carlo simulation was used to see the movement of the price. Initially I just simulated the stock price movement by calculating the returns using the log formula and then calculating the price through exponential function. I also simulated the volatility to see the deviance in the stock. Ultimately, I made a regression model to predict the prices and assessed its fit. A Monte Carlo simulation can also determine the size of the portfolio a client would need at retirement, to support their desired retirement lifestyle. I then, determined the expected value and distribution of the portfolio at the retirement age. The model requires some prior hypotheses. I assumed that the daily returns of these assets are normally distributed with mean(μ), and standard deviation sigma, (σ). To compute μ, which is the mean of the daily returns, I took n successive past close prices and applied, which is the average of the sum of the n past prices. I computed the volatility also from n past closed prices by the standard deviation formula. Annualized volatility was calculated by multiplying with the sqrt of the number of trading days.
 
Reference Links-
https://www.investopedia.com/articles/investing/102715/simulating-stock-prices-using-excel.asp
https://www.kaggle.com/camnugent/sandp500

