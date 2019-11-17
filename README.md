# Project Motivation
Investment banks, hedge funds — even individual investors — develop financial models to predict price movements in publicly-traded securities. Successfully anticipating these movements can prove highly profitable for the investor; at the same time, a misstep could spell financial ruin. Historical stock prices provide a treasure trove of data, which may be suitable for machine learning algorithms to predict future stock price movements and — ultimately — drive more well-informed investment decisions. In this work, we build a stock price predictor that predicts stock price movements — specifically whether a price will rise or fall — based on historical performance.  To do so, data were pulled from Yahoo Finance (https://finance.yahoo.com/) for a number of stock tickers along with an ETF that indexes the S&P 500.

# Project Write-up
A blog post detailing the approach to this analysis and the results can be found here: https://medium.com/@aaron.chockla/no-you-cant-predict-stock-prices-but-can-you-predict-price-movements-1a2757e55967

# Key Questions Addressed
* Can the movement in stock prices (*i.e.*, rise or fall in price, rather than predicting a specific price) be predicted with reasonable accuracy?
* Does such accuracy very by ticker or sector?
* How far into the future can such price movements be predicted while maintaining accuracy?

## Project Files
* **Stock csv files** contain historical stock pricing data (Open, High, Low, Close, Adjusted Close, and Volume) for six separate stocks and an index fund.
* **Capstone Project.ipynb** python notebook for processing and analyzing the stock data.
* **Capstone Project.html** contains an html version of the python notebook.

## Dependencies
* **Python:** Python 3+ (I used Python 3.7)
* **Data Analysis Libraries:** NumPy, SciPy, Pandas, Sciki-Learn
* **Other Utility Libraries:** matlotlib, datetime

## Summary of Analysis
**1.** Publicly available historical stock pricing data can be used to generate a machine learning model that *can* predict whether a stock price will trend up or down over a period of one day to one month into the future.

**2.** Prediction accuracy is better than employing a unilateral strategy (that stock prices will always increase, for example).

**3.** Prediction accuracy falls when looking out further than 4trading periods into the future.

**4.** This approach does not predict stock prices and therefore does not inform trading strategies.

## License
This project is licensed under the MIT License - see the [LICENSE] (https://github.com/AaronChockla/DisasterResponse/blob/master/LICENSE) file for details.

## Acknowledgement
* Yahoo Finance for making these data publicly available
* Various addtional resources cited in the ipynb file
