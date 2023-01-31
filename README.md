# Introduction

This script contains code to process and analyze a financial data set. The data set includes several columns of information, including information about the prices of different cryptocurrencies, market indices, and more. The data is stored in an Excel spreadsheet and is loaded into a Pandas dataframe for processing.


# Prerequisites

Before running this script, you must have the following libraries installed:

+ pandas
+ numpy
+ matplotlib
+ tensorflow
+ scikit-learn

# Data Processing

The data is loaded from an Excel spreadsheet into a Pandas dataframe using the pd.read_excel function. The resulting dataframe has 4501 rows and 16 columns. The data is stored with a DatetimeIndex to make it easy to work with time-series data.

The data includes information about the following:

+ Bitcoin price
+ BTC network difficulty
+ Bitcoin circulation
+ All BTC transactions
+ BTC transactions over 100000$
+ Ethereum price
+ BTC hash rate
+ Active addresses
+ ATM for crypto
+ VIX index
+ DXY index
+ Gold price
+ Telegram positive sentiments
+ Telegram negative sentiments
+ Twitter positive sentiments
+ Twitter negative sentiments

# Correlation Analysis

The correlation between the columns in the dataframe is calculated using the data.corr() function. This can help identify which columns are strongly related to each other and may be useful in building a predictive model.

# Predictive Modeling

The script includes code to build a predictive model using TensorFlow and the Keras API. The model is built using a Sequential model and includes the following layers:

+ Flatten
+ BatchNormalization
+ LSTM
+ Dropout
+ Dense

The model is trained using a sliding window approach to generate inputs and targets from the data. The sliding window size is specified by the user and the inputs are normalized using the MinMaxScaler from scikit-learn. The model is trained using mean squared error as the loss function.

# Conclusion

This script provides a basic framework for analyzing financial data and building a predictive model for cryptocurrency prices. With further modification, this script could be used as the basis for a more comprehensive analysis or trading strategy.

![image](https://user-images.githubusercontent.com/95343201/215766409-64648600-9aca-4053-bc4d-1d986bf8f508.png)
