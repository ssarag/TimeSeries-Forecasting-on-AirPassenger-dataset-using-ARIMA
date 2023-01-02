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

# Checking if the dataset is Stationary

![image](https://user-images.githubusercontent.com/103538049/210274086-7a40675a-b324-45d3-801e-bb6d67753c19.png)


# Rolling Statistics

![image](https://user-images.githubusercontent.com/103538049/210274145-a4cd57ca-bc50-4c50-bb81-a53ab2908b20.png)


# Checking if the data is stationary by performing Augumented Dickey-Fuller Test

![image](https://user-images.githubusercontent.com/103538049/210274221-f71976d0-93da-4bcc-a301-adaa6f095654.png)


As the value of p is greater than 0.05, we can confirm the data is not stationary. To make the data stationary, next we will perform the decomposition of data. 


# Sesonal Decomposition

![image](https://user-images.githubusercontent.com/103538049/210274316-5e68a3fd-f301-4047-aafb-7daa32c52919.png)


# Finding the value of the d paramete



![image](https://user-images.githubusercontent.com/103538049/210274585-a77689ed-8b7e-443d-9c25-3d82363c786c.png)

