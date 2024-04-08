# Bitcoin Investment Strategy
This repository provides a code implementing an investment strategy on Bitcoin based on the halving process. The project can be divided into 3 main parts:
* Time series analysis of Bitcoin
* Development of a Monte Carlo simulation
* Evaluation of a European Option by means of the Monte Carlo simulation
## Description
For the sake of this project, it is essential to explain briefly how the Bitcoin halving works: every miner receives a compensation in Bitcoins for every block it is able to mine; by default, this reward gets reduced by half every 210000 blocks (which is equivalent to a period of approximately 4 years). Historically, this event leads Bitcoin to reach a new all time high within 1 year from it, this observation is shown in the statistical analysis carried out in the code.

Afterwards, the ARIMA Model and the GARCH Model were applied: the former is used to forecast the future values of a time series by using past data, while, the latter is employed to analysis the element of volatility. Unfortunately, both models gave poor results given the frequent fluctuations of the asset. Therefore, a simple model was developed by determining the average return of Bitcoin before and after each halving using the volume as weight; through this model, a forecast for the price of Bitcoin can be obtained in the 1-year and 2-years periods after the 2024 halving.

Afterward, a Monte Carlo simulation is carried out in order to obtain plausible forecasts for the price and the return of Bitcoin.

Finally, the Black-Scholes-Merton model is used to price a European call option on Bitcoin.
## Softwares
Python was the only software used to code this project.
## Credits
* Giovanni Anghinoni <anghinonigiova@gmail.com>
* Emrecan Türkmen <emrecanturkmen@gmail.com>
## References
Hilpisch, Y. J. (2018). Python for Finance. O’Reilly.

Cryer, J. D., Chan, K. (2008). Time Series Analysis. Springer.
## Remarks
This research was carried out between April and July 2023, therefore, more recent events, i.e. the approval of the first 11 Bitcoin ETFs by the SEC in 2024, which caused billions of dollars to flow into Bitcoin leading to an earlier than expected new all time high, could have not been taken into account. The market of cryptocurrencies is rapidly evolving and even a small piece of information can influence it greatly; consequently, research must be realized continuously and kept updated.
