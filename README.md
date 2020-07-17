# Time series Analysis
Data used in the Notebooks can be found here : https://archive.ics.uci.edu/ml/datasets/Metro+Interstate+Traffic+Volume

Explorary Data Analysis : univariate analysis, seasonality and correlations

Benchmarking of different Algorithms used for forecasting : 

| Algorithms               	| Train Error 	| Test Error 	|
|--------------------------	|-------------	|------------	|
| ARIMA                    	|      -      	|   644.08   	|
| Prophet                  	|      -      	|    817.7   	|
| Prophet with regressor   	|      -      	|   817.63   	|
| Prophet with all feature 	|      -      	|   814.09   	|
| Vanilla LSTM             	|     466     	|   513.82   	|
| Stacked LSTM             	|    460.47   	|   513.86   	|
| Bidirectional LSTM       	|    438.07   	|   488.19   	|
