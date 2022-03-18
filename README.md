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

| Algorithm                    	| Training Time 	| Forecasting Time 	| RMSE   	| MAE    	| MAPE    	|
|------------------------------	|---------------	|------------------	|--------	|--------	|---------	|
| ARIMA                        	| 638 ms        	| 1min 11s         	| 542.68 	| 394.21 	| 23.61 % 	|
| Prophet (baseline)           	| 2.6 s         	| 2.01 s           	| 985.96 	| 755.68 	| 40.36 % 	|
| Prophet (1 regressor)        	| 1.87 s        	| 2.2 s            	| 842.02 	| 636.90 	| 37.79 % 	|
| Prophet (4 regressors)       	| 1.09 s        	| 2.16 s           	| 837.53 	| 626.79 	| 36.02 % 	|
| Prophet (optimized)          	| 31.4 s        	| 2.57 s           	| 380.87 	| 293.86 	| 18.40 % 	|
| LSTM                         	| 1min 31s      	| 628 ms           	| 613.44 	| 426.53 	| 14.62 % 	|
| XGBoost (only time features) 	| 1.81 s        	| 9 ms             	| 311.21 	| 213.37 	| 12.48 % 	|
| XGBoost (all features)       	| 3.02 s        	| 6.99 ms          	| 281.19 	| 181.95 	| 9.68 %  	|
| XGBoost (fine tuned)         	| 5.64 s        	| 5 ms             	| 277.48 	| 181.79 	| 8.00 %  	|