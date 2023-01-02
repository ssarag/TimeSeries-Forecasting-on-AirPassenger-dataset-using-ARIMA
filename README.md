# Time Series Forecasting ARIMA Model

The main objective of this project is to use ARIMA model for time series forecasting. 

# Dataset used:

For this project, the AirPassenger dataset is used. This dataset provides monthly totals of US airline passengers from 1949 to 1960. 

# To implement the model, the below 4 essential steps are used

Step 1 --->  Check Stationarity: 
If a time series has a trend or seasonality component, it must be made stationary.

Step 2 ---> Determine the d value: 
If the time series is not stationary, it needs to be stationarized through differencing.

Step 3 --> Select AR and MA terms: 
Use the ACF and PACF to decide whether to include an AR term, MA term, (or) ARMA.

Step 4 ---> Build the model

# Results

In the inital step, the dataset is loaded into pandas csv file. There are 2 columns in the dataset, 'Date' and 'Passenger'. In the date colukn, I have applied pythom's datetime function to convert the dates in the required format. Below is how the dataset looks after processing. 


![image](https://user-images.githubusercontent.com/103538049/210273982-289496ac-bd76-45c1-a9cb-57f0a06572d2.png)

