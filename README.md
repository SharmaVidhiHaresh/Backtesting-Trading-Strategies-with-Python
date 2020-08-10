# Backtesting-Trading-Strategies-with Python
We would backtest the cross-over trading strategy on Google Stock from Jan 2016 to June 2020.
By using historical data, we can test the returns and risk of the employing Moving Average(MA) cross-over strategy and Relative Strength Index (RSI) strategy under various market conditions.

<img src="/Pricing chart with technical indicator.png" >

# Premises of the strategy

### Relative Strength Index (RSI)
The relative strength index (RSI) is a momentum indicator used in technical analysis that measures the magnitude of recent price changes to evaluate overbought or oversold conditions in the price of a stock or other asset.
Traditional interpretation and usage of the RSI are that values of 70 or above indicate that a security is becoming overbought or overvalued and may be primed for a trend reversal or corrective pullback in price. An RSI reading of 30 or below indicates an oversold or undervalued condition.

### Moving Average (MA) Crossover
The shorter the time span used to create the average, the more sensitive it will be to price changes. The longer the time span, the less sensitive the average will be.
upward momentum is confirmed with a bullish crossover, which occurs when a short-term moving average crosses above a longer-term moving average. Conversely, downward momentum is confirmed with a bearish crossover, which occurs when a short-term moving average crosses below a longer-term moving average.

## Setting the stop-loss:
If the price closes 2% or more below 10-day MA, close the position, if any.

## Trade Set-Up
#### Buy the position when:
 * weekly RSI(30)  ≥  daily RSI(30)  >  70
 * Close  >  MA(10)  >  MA(20)  >  MA(50)  >  MA(100)
#### Close the position when:
 * Daily close is more than 2% below MA(10)
 * 8% fixed stop loss is hit



