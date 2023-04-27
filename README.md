# Challenge VI | PyViz Visualization Tools |Fintech <img src="https://instructure-uploads-pdx.s3.us-west-2.amazonaws.com/account_150420000000000001/attachments/590996/columbia.png" height="48" width="48">

---

This is the 5th challenge, now for Financial Planning based on data taken from APIs and simulations
The idea is to analyze and validate the different scenarios for a portfolio for a 10 year and 30 year horizon

The current portfolio contains a combination of the following componentns: 

- **STOCKs (ETF) $SPY (S&P 500 ETF)**            
- **Bonds $AGG (Shares Core US Aggregate Bond ETF)**    
- **Crypto Currencies (ETH & BTC)**    


Information is obtained from the following APIs: 

- [Alpaca API](https://alpaca.markets/)
- [BTC Ticker](https://api.alternative.me/v2/ticker/Bitcoin/?convert=USD)
- [ETH Ticker](https://api.alternative.me/v2/ticker/Ethereum/?convert=USD)

---

## Libraries Used

The main language is Python embeded in Jupyter lab

### jupyter

This modules creates a notebook and processes a python kernel.

### pandas

Library that handles Dataframes and Series to process data, filter, create statistics

### matplotlib

Library to plot graphs

### alpaca_trade_api

This is and SDK provided by Alpaca Markets to abstract the API logic into Python classes.

### dotenv

Library used to load, read and process environment variable files.

## json

Library used to process JSON text coming from the APIs, also formats and reprocess JSONs to convert it into a Python Dictionary

## requests

Library to process HTTP Requests and send the different HTTP Requests methods,

## os

Library for Operating System functionalities, particularily, processing Environment variables into Python.

## MCSimulation

Custom made library provided by Columbia to generate a light Monte Carlo Simulation with common libraries (NumPy and Pandas)

---

## Usage

To run program just open the terminal (anaconda needs to be installed) and type the following

``` bash
$ git clone https://github.com/lumiroga/fintech-Challenge5.git
$ cd fintech-Challenge5
$ jupyter lab 

```

Open a browser with the displayed URL in Jupyter

Look for *risk_return.ipnyb* file and open it.

---
# Analysis Description -  Financial Planning

The process is divided into 2 parts, first analyzing the current value of the portfolio, getting the most recent data to calculate the values.

## Get Emergency Fund

Considering a monthly income of 12 thousand USD, an emergency fund should at least cover 3 months of income.

### Get Current Values for Crypto Currency

Using API Alternative Ticker we get the latest values for ETH and BTC to calculate the current value in dollars for the given portfolio

### Get Current Values for Stocks and Bonds

Using Alpaca API we get the latest values for $AGG and $SPY to calculate the current value in dollars for the given portfolio

## Evaluate Emergency Fund

Check if the current value combining the Cryptocurrencies, Stocks and Bonds is enough for an emergency fund (3 months of income)

## Financial Planner

Using the MCForecastTools Library, we calculate the estimated value and expected value for the Stock and Bond portfolio

### 30 Years Simulation

The 30 years simulation gives an overall estimated value with 95% confidence of between $117k to $1.4M 

### 10 year Simulation

The 10 years simulation gives an overall estimated value with 95% confidence of between $71k to $435k 

## Contributors

[lumiroga](https://github.com/lumiroga)

---

## License

* mpl-2.0 | Mozilla Public License 2.0