# Time series Analysis
Data used in the Notebooks can be found here : https://archive.ics.uci.edu/ml/datasets/Metro+Interstate+Traffic+Volume


### Data Set Information:

Hourly Interstate 94 Westbound traffic volume for MN DoT ATR station 301, roughly midway between Minneapolis and St Paul, MN. Hourly weather features and holidays included for impacts on traffic volume.


#### Attribute Information:

- holiday Categorical US National holidays plus regional holiday, Minnesota State Fair
- temp Numeric Average temp in kelvin
- rain_1h Numeric Amount in mm of rain that occurred in the hour
- snow_1h Numeric Amount in mm of snow that occurred in the hour
- clouds_all Numeric Percentage of cloud cover
- weather_main Categorical Short textual description of the current weather
- weather_description Categorical Longer textual description of the current weather
- date_time DateTime Hour of the data collected in local CST time
- traffic_volume Numeric Hourly I-94 ATR 301 reported westbound traffic volume



### Explorary Data Analysis :
univariate analysis, seasonality and correlations

### Benchmarking of different Algorithms used for forecasting : 

| Algorithms               	| Train Error 	| Test Error 	|
|--------------------------	|-------------	|------------	|
| ARIMA                    	|      -      	|   644.08   	|
| Prophet                  	|      -      	|    817.7   	|
| Prophet with regressor   	|      -      	|   817.63   	|
| Prophet with all feature 	|      -      	|   814.09   	|
| Vanilla LSTM             	|     466     	|   513.82   	|
| Stacked LSTM             	|    460.47   	|   513.86   	|
| Bidirectional LSTM       	|    438.07   	|   488.19   	|
