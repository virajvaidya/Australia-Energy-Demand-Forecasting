#  :bulb: Australia Energy Demand Forecasting :zap:

This repository consists of a SARIMA (Seasonal Autoregressive Integrated Moving Average) forecasting model in Python to predict electricity demand in NSW, VIC, QLD, TAS and SA.

I have downloaded, cleaned and put together into CSV files electricity demand and electricity price data comprising of over a million data points from AEMO to build a pipeline that automates the (p,d,q) selection for the SARIMA model and outputs forecast values using the best fitting model (using the Bayesian Information Criterion).

For the period between 01-01-2019 and 31-12-2020, frequency of observations is every 30 minutes.
Fore the period after that until 19-12-2021, the frequency of observations is every five minutes.

I have chosen to go with an autoARIMA automated pipeline in Python’s pmdarima package. An advantage of using this particular package is that it presents the option of incorporating a seasonal decomposition using a Fourier Transform into the pipeline itself using the Fourier-Featurizer function, which means that the seasonal decomposition of the data doesn’t need to be done separately manually.


I have split up the Python scripts into a preliminary Exploratory Data Analysis (AEMODATAEDA) file and individual forecast files (in the interest of lightness)  for each of the five states.

As always, comments, feedback are welcome.

