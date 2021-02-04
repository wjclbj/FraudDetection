# FraudDetection
Fraud Detection using both supervised/unsupervised learning

## Story
A project trying to detect transaction anomalies using supervised/unsupervised learning algos. (XGBoosting, Isolation Forest, and Local Outlier Factor)

## Dataset
[Synthetic Financial Datasets For Fraud Detection](https://www.kaggle.com/ntnu-testimon/paysim1/data)

- Context
There is a lack of public available datasets on financial services and specially in the emerging mobile money transactions domain. Financial datasets are important to many researchers and in particular to us performing research in the domain of fraud detection. Part of the problem is the intrinsically private nature of financial transactions, that leads to no publicly available datasets.

We present a synthetic dataset generated using the simulator called PaySim as an approach to such a problem. PaySim uses aggregated data from the private dataset to generate a synthetic dataset that resembles the normal operation of transactions and injects malicious behaviour to later evaluate the performance of fraud detection methods.

- Content
PaySim simulates mobile money transactions based on a sample of real transactions extracted from one month of financial logs from a mobile money service implemented in an African country. The original logs were provided by a multinational company, who is the provider of the mobile financial service which is currently running in more than 14 countries all around the world.

This synthetic dataset is scaled down 1/4 of the original dataset and it is created just for Kaggle.

## Evaluation

1. XGBoosting

|              	| precision 	| recall 	| f1-score 	| support 	|
|--------------	|-----------	|--------	|----------	|---------	|
| 0            	| 1.00      	| 0.99   	| 1.00     	| 552439  	|
| 1            	| 0.28      	| 0.99   	| 0.44     	| 1643    	|
| accuracy     	| 0.99      	| 554082 	|          	|         	|
| macro avg    	| 0.64      	| 0.99   	| 0.72     	| 554082  	|
| weighted avg 	| 1.00      	| 0.99   	| 0.99     	| 554082  	|

2. Isolation Forest

|              	| precision 	| recall 	| f1-score 	| support 	|
|--------------	|-----------	|--------	|----------	|---------	|
| 0            	| 1.00      	| 1.00   	| 1.00     	| 552439  	|
| 1            	| 0.05      	| 0.05   	| 0.05     	| 1643    	|
| accuracy     	| 0.99      	| 554082 	|          	|         	|
| macro avg    	| 0.52      	| 0.52   	| 0.52     	| 554082  	|
| weighted avg 	| 0.99      	| 0.99   	| 0.99     	| 554082  	|

3. LOF

|              	| precision 	| recall 	| f1-score 	| support 	|
|--------------	|-----------	|--------	|----------	|---------	|
| 0            	| 1.00      	| 1.00   	| 1.00     	| 552439  	|
| 1            	| 0.02      	| 0.02   	| 0.02     	| 1643    	|
| accuracy     	| 0.99      	| 554082 	|          	|         	|
| macro avg    	| 0.51      	| 0.51   	| 0.51     	| 554082  	|
| weighted avg 	| 0.99      	| 0.99   	| 0.99     	| 554082  	|
