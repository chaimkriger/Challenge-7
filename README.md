# *ETF Analyzer Application*

In the ETF Analyzer Application, i complete an analysis of a fintech ETF that consists of four stocks: GOST, GS, PYPL, and SQ. Each stock has its own table in the etf.db database, which the Starter_Code folder contains.

i Analyze the daily returns of the ETF stocks both individually and as a whole. i then deploy the visualizations to a web application by using the Voilà library.

The Application is divided into the following parts:

Analyze a single asset in the ETF.

Optimize data access with advanced SQL queries.

Analyze the ETF portfolio.

Deploy the notebook as a web application.


I start off by analyzing a single asset in the ETF: Paypal. I write a SQL SELECT statement that reads all the PYPL data from the database. I then use that statement to execute a query that reads the PYPL data from the database into a Pandas DataFrame. Using hvPlot, i create an interactive visualization for the PYPL daily returns, and the PYPL cumulative returns.

I then optimize data access with advanced SQL queries. I first access the closing prices for PYPL that are greater than 200 by writing a SQL SELECT statement to select the dates where the PYPL closing price was higher than 200.0. Using the SQL SELECT statement, i can then read the data from the database into a Pandas DataFrame, and review the resulting DataFrame. Lastly, i find the top 10 daily returns for PYPL by writing a SQL statement to find the top 10 PYPL daily returns. 

The next task is to Analzye the ETF portfolio as a whole. To start, i build the ETF portfolio by using SQL joins to combine all the data for each asset.
I write a SQL query to join each table in the portfolio into a single DataFrame. Using the SQL query, I read the data from the database into a Pandas DataFrame. I then create a DataFrame that averages the “daily_returns” columns for all four assets. I use the average daily returns in the etf_portfolio_returns DataFrame to calculate the cumulative returns of the ETF portfolio. And finally, i use hvPlot to create an interactive line plot that visualizes the cumulative return values of the ETF portfolio. 

The final step in my ETF analyzer application is to deploy the notebook as a web application. To do so, i use the Voilà library. Ive taken screenshots to show how the web application appears when using Voilà and included them in my README.md file 

---

## Technologies

This project leverages Python 3.7.

---

## Installation Guide

Before running this application, Python must be installed.

---

## Usage
 
To run the ETF Analyzer Application, simply pull the code and run it. You are free to edit any of the query's to your own preferences.
Attached below are some screeshots from my voila webpage.


![Screenshot of Paypal cumulative returns over 4 years](https://github.com/chaimkriger/Challenge-7/blob/main/2021-10-31%20(1).png)
![Screenshot of my sql query that joined the 4 tables together](https://github.com/chaimkriger/Challenge-7/blob/main/2021-10-31%20(2).png)
![Sceenshot of etf cumulattive returns over 4 years](https://github.com/chaimkriger/Challenge-7/blob/main/2021-10-31%20(3).png)

---

## Contributors

Just me, and a little bit of help from module 7

## License

No license, feel free to copy the code any time.
