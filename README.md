# Time_Series_Analysis
The time series analysis forecasts historic daily returns for the Yen currency. I trimmed my data to begin on January 1st 1990. 
I then plotted the settlement price for my data set.The plot showed a long-term strengthening of the Japanese Yen against the Dollar. There do seem to be some more medium, 1-3 year consistent trends, but on a daily basis, there are a lot of short-term ups and downs.
I then used the Hddrick-Prescott Filter to decompose the data into noise and trend series.Smoothing with the HP Filter and plotting the resulting trend against the actual futures returns, we can see that there's a lot of short term fluctuations that deviate around this trend. Perhaps these would represent profitable trading opportunities.
I then forcasted the returns using the ARMA model, and determined that my model was not a good fit. the coeifficient did not appear to be statistically significant. 
I then forcasted the settlement price using an ARIMA Model. The model forecasted that the price of the Yen will climb in the near term. 
I then Forecasted the volitility using the GARCH model. The model forecasted increasing volitilty in the near term. 
# Conclusions
Based on my time series analysis I would not buy the yen now. Although the price is projected to rise in the coming 5 days, this comes with the risk of increased volitilty. I also question the validity of the models used to come up with these results, since only one coefficient in my GARCH model would be considered statistically significant(a1<.05). All other models have no statistically significant coefficients.
The risk of the yen is expected to increase over the next 5 days. We can determine this by looking at the 5 day forecast of viotility. However higher volatility leads to more risk which can lead to higher returns.
Based on the model evaluation I would not feel confident using these models for trading. Both models have p scores larger than .05 showing no statistical significants. 
 
 # regression_analysis
I used Regression Analysis to determine Seasonal Effects with SKlearn Linear Regression 
I first trimmed the data to begin on January first 1990.
I then calculated a percentage change and lagged return.
I then train, tested and split my data.
I then made both out of sample and in sample predicitions using the testing data 
 # Conclusions
I determined This model performs better on the out of sample data. We can infer this because the RMSE is .41 for the out of sample data and .57 for the in smaple data. 
 
