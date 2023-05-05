# linear_Regression_ETHUSDT_BTCUSDT
Removing the Effect of BTC on ETH Prices in API Applications using Correlation Analysis and Residual Calculation

_This project aims to provide developers with a methodology to remove the effect of BTC on ETH prices in API applications. By implementing the methodology outlined in this project, developers can ensure that the ETH prices served in their API applications are independent of changes in BTC prices._

## The methodology involves the following steps:

1-Correlation Analysis: The correlation between BTC and ETH prices is calculated using linear regression. 
_This step is necessary to understand the relationship between the two variables._

2-Residual Calculation: The predicted ETH prices based on the BTC prices are subtracted from the actual ETH prices to obtain the residuals.
_The residuals represent the changes in ETH prices that are not explained by changes in BTC prices._

3-Second Linear Regression: A second linear regression is performed between the residuals and the actual ETH prices to find the line of best fit between the two variables. 
_This regression line represents the changes in ETH prices that are not affected by changes in BTC prices._

4-Residual Prediction: The ETH prices based on the residuals are predicted, and the predicted values are subtracted from the actual ETH prices. The resulting values represent the changes in ETH prices that are not explained by changes in BTC prices, and therefore, the effect of BTC on ETH prices is removed.

5-The data used in the code was extracted from the symbols "ETH" and "BTC" using the CoinMarketCap API. The API endpoint used to obtain the latest quotes for these symbols was ("https://pro-api.coinmarketcap.com/v1/cryptocurrency/quotes/latest"). The API key was set in the headers of the request using the "X-CMC_PRO_API_KEY" parameter. The "Accepts" parameter was also set to "application/json" to indicate that the API should return data in JSON format.


Note :_This methodology is simple and there are alote of more complexed methods , but this method can be implmented efficiently in API applications by incorporating the code provided in this project. The scikit-learn library is used to perform the linear regression, and the default parameters are used in the implementation._

