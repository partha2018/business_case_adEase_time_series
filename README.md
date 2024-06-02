# business_case_adEase_time_series


## Ad Ease website Analytics
### Dataset: Web Traffic Time Series Forecasting

Forecasting the future values of multiple time series. More specifically the problem of forecasting future web traffic for approximately 145,000 articles on britanica.

The training dataset consists of approximately 145k time series. Each of these time series represent a number of daily views of a different article, starting from July, 1st, 2015 up until December 31st, 2016. For each time series, you are provided the name of the article as well as the type of traffic that this time series represent (all, mobile, desktop, spider). You may use this metadata and any other publicly available data to make predictions. Unfortunately, the data source for this dataset does not distinguish between traffic values of zero and missing values. A missing value may mean the traffic was zero or that the data is not available for that day.

### Data Dictionary:

there are two csv files given

*train_1.csv : *

In the csv file, each row corresponds to a particular article and each column correspond to a particular date. The values are the number of visits in that date.

*Exog_Campaign_eng : *

this file contaings data for the dates which had a campaign or significant event that could affect the views for that day. the data is just for pages in english.

there is a 1 for dates with campaign and 0 for remaining dates. It is to be treated as an exogenous variable for models when training and forecasting data for pages in english

### Intent of the notebook
We will start by loading the data and handling the values.

Then some Exploratory data analysis to get an understanding of the data and get some useful insight, based on various parameters, and visualizing them.

Preparing the data for feeding to the model(checking stationarity, transformations).

Preparing the model followed by some predictions.

Comparing the same with the given data and calculating the accuracy of the model.
