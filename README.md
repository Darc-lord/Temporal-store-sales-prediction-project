# Temporal-store-sales-prediction-project
A machine Learning project aimed at making temporal predictions, predicting the daily sales of product families in all `Ecuadorian Corporación Favorita stores` in the month of August 2017 using time as the main predictor component and given other key features such as store information, holiday dates, Oil prices,etc.

## Table of contents
+ Project Overview
+ Installation
+ Files
+ Acknowledgement

### Project Overview
The project was done for submission in the Kaggle **Store Sales - Time Series Forecasting competition** . The objectives of this challenge is to use times series forecasting to predict store sales on data from Corporación Favorita, a large Ecuadorian-based grocery retailer. The evaluation metric the competition body required was Root Mean Squared Logarithmic Error (RMSLE).
The steps taking in creating the model:

- **Exploratory Data Analysis**: Which involves going through the data, it's columns and it's rows checking for missing data, correlation, relationships and patterns, trends, seasonality and cycles.
- **Filling Missing Data**: This is a crucial part of the model creation purpose, Models cannot thoroughly learn from Nan values. The method of filling is crucial, as you could distort the temporal nature of the data if not filled properly.
- **Feature Engineering**: This is a very important aspect of time series forecasting as you have to engineer time series features that your model can understand. `Scikit-Learn` has a method to achieve this using DeterministicProcess and CalenderFourier, to create trend, seasonal and cyclic features. Engineering holiday features and other features also add to your models databank.
- **Converting categorical data into Numerical form and encoding them**: As the intro says,this section involves converting all categorical and all object dtypes into Numerical dtypes. This is crucial as Machine learning Models only learn from Numerical data.
- **Modelling**: This section involving applying machine learning models to our already clean datase. In this project LogisticRegression, Xgboost Regressor and Ensemble's Random Forest Regressor were both evaluated and tuned to find which found more pattern and learned better on the data. A hybrid model was also created using LogisticRegression and Xgboost as both models would learn different parts of the data and their predictions combined to form the submitted prediction
  
### Installation
1. **Anaconda**
	```bash
	 https://www.anaconda.com/download
	```

### Files
1. **Clone The Repository**
	```bash
	git clone https://github.com/Darc-lord/Temporal-store-sales-prediction-project.git
	cd Insurance-Premium-Amount
	```

2. **Download Dataset**
	```bash
	 [https://www.kaggle.com/competitions/playground-series-s4e12/data](https://www.kaggle.com/competitions/store-sales-time-series-forecasting/data)
	```	

## Acknoledgements
+ Kaggle
+ Playground Series
+ Scikit-learn

