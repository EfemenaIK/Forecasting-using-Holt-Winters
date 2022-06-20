# Forecasting-using-Holt-Winters
The Holt-Winters method — also known as TRIPLE exponential smoothing — is an incredibly popular and relatively simple method for time series forecasting. 
Holt-Winters Exponential Smoothing is used for forecasting time series data that exhibits both a trend and a seasonal variation.

The Holt-Winters method is a very common time series forecasting procedure capable of including both trend and seasonality. The Holt-Winters method itself is a combination of 3 other much simpler components, all of which are smoothing methods:

#### 1. Simple Exponential Smoothing (SES): 
Simple exponential smoothing assumes that the time series has no change in level. Thus, it can not be used with series that contain trend, seasonality, or both. The simple exponential smoothing method does not take into account any trend or seasonality. Rather, it assumes that the time series data only has a level, L.

<img width="150" alt="image" src="https://user-images.githubusercontent.com/58333385/174688730-ee9cb48f-8459-4886-9602-9facbcc95b4d.png">

This equation is known as the level update equation, as it updates the level of the current time step based on the previous level estimate.

#### 2. Holt’s Exponential Smoothing (HES): 
Holt’s exponential smoothing is one step above simple exponential smoothing, as it allows the time series data to have a trend component. Holt’s exponential smoothing is still incapable of cope with seasonal data.
Holt’s method extends simple exponential smoothing by assuming that the time series has both a level and a trend. 

<img width="103" alt="image" src="https://user-images.githubusercontent.com/58333385/174689055-1532ccf0-54b7-417f-928d-87759273eb00.png">

As we can see, it is literally just a simple extenuation of original SES method, just with the inclusion of the trend, T, component.

However, it is important to note that there are two types of time series, each with their own slightly different forecasting equation:

- Additive: In an additive time series, the time series is the sum of its components.
- Multiplicative: In a multiplicative time series, the time series is the product of its components.

#### 3. Winter’s Exponential Smoothing (WES): 
Winter’s exponential smoothing is an extension to Holt’s exponential smoothing that finally allows for the inclusion of seasonality. Winter’s exponential smoothing is what is referred to as the Holt-Winters method.
Since Winter’s exponential smoothing is built on top of both single and double exponential smoothing, Winter’s method is thus also known as triple exponential smoothing. Winter’s method assumes that the time series has a level, trend and seasonal component.







