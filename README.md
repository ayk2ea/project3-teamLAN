# Project 3: Predicting AMC Stock Outcomes using Autoregression - Team LAN
## Repository Contents 

## SRC
### Installing/Building the Code
In order to conduct a time series study of data on the past 10 years of AMC stock values, an Autoregressive Integrated Moving Average (ARIMA) model was used. This model uses time series data to forecast upcoming data points. There are two functions in the forecast package for making such a model. The auto.arima() function creates multiple variations of the model to create the best fit, while the arima() function allows for manual input of parameters. 
For this project, we used the ARIMA code to manually choose p, d, and q and to incorporate seasonality. 


### Code Usage
Using the code found in the SRC folder, run the file titled ______. Ensure that the following packages have been installed: fpp, forecast. This file will use the ARIMA function on the cleaned dataset, AMCdataFinal.csv (found in the Data folder) to create a projection of the stock prices for the next 12 months to identify the best time to sell AMC stocks. 


## Data
### Data Dictionary
| Column | Data Type | Description |
| --- | --- | --- |
| Date | Character | Date corresponding to data |
| Close/Last | Character | Adjust consolidated close stock price provided in USD |
| Volume | Integer | Number of shares traded within the day |
| Open | Character | Price of first stock transaction made for a date |
| High | Character | Highest transaction value for the day |
| Low | Character | Lowest transaction value for the day |

### Link to Data
https://www.nasdaq.com/market-activity/stocks/amc/historical 

### Notes about Data

Use dataset [AMCdataFinal.csv](https://github.com/ayk2ea/project3-teamLAN/blob/main/DATA/AMCdataFinal.csv) for cleaned data.

## Figures 

| Figure | Image | Description|
| --- | --- | --- |
| ARIMA Residuals | ![ARIMA Residuals](/FIGURES/ARIMAResiduals.jpeg) | Residual plots displaying what's left over after fitting the time series model |
| Box Test | ![Box Test](/FIGURES/BoxTest.jpeg) | Box-Ljung test applied to the residuals from the ARIMA model fit to determine for randomness |
| Forecasts Graph | ![Forecasts Graph](/FIGURES/new arima prediction.jpeg) | Plot displaying forecasts for AMC stock |

## References

“AMC Theaters is changing its ticket pricing,” CNN Business. [Online]. Available: https://www.cnn.com/2023/02/06/business/amc-movie-ticket-prices/index.html. [Accessed: 4-Apr-2023].

“Top Meme Stocks and Meme Stock Rallies,” Forbes. [Online]. Available:
https://www.forbes.com/sites/qai/2022/09/02/top-meme-stocks-and-meme-stock-rallies/?sh=6ee5f5591b24. [Accessed: 4-Apr-2023].

“What Is ARIMA Modeling?,” Masters in Data Science, 04-Aug-2022. [Online]. Available: https://www.mastersindatascience.org/learning/statistics-data-science/what-is-arima-modeling/. [Accessed: 04-Apr-2023]. 

“How to Create an ARIMA Model for Time Series Forecasting in Python,” Machine Learning Mastery. [Online]. Available: https://machinelearningmastery.com/arima-for-time-series-forecasting-with-python/. [Accessed: 4-Apr-2023]. 

“Time Series Analysis using ARIMA model in R Programming,” Geeks for Geeks. [Online]. Available: https://www.geeksforgeeks.org/time-series-analysis-using-arima-model-in-r-programming/. [Accessed: 11-Apr-2023].

“Time Series - ARMA Models in R,” RPubs. [Online]. Available: https://rpubs.com/JSHAH/481706. [Accessed: 11-Apr-2023].

“Lesson 3: Identifying and Estimating ARIMA models; Using ARIMA models to forecast future values,” STAT ONLINE Penn State. [Online]. Available:
https://online.stat.psu.edu/stat510/book/export/html/665. [Accessed: 11-Apr-2023].

“Interpreting ACF and PACF Plots for Time Series Forecasting,” Towards Data Science, 02-Aug-2022. [Online]. Available: https://towardsdatascience.com/interpreting-acf-and-pacf-plots-for-time-series-forecasting-af0d6db4061c. [Accessed: 11-Apr-2023].
