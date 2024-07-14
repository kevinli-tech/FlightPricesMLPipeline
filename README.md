# Flight Prices Prediction
This repository contains the project "Flight Prices Prediction," which aims to predict future flight prices based on historical data using machine learning techniques.<br />

## Introduction
The project focuses on predicting flight prices using a dataset obtained from Kaggle. The objective is to develop a predictive model to assist travelers in optimizing travel expenses.<br />

## Dataset
The dataset titled "Flight Prices" can be found on Kaggle. It contains various attributes related to flights, such as departure city, destination city, airline, departure date, arrival date, and price.<br />

### Data Analysis and Cleaning
Null values were dropped, and irrelevant columns were removed to improve the dataset quality. Specifically, columns with high cardinality or those irrelevant to the model's objective were excluded to enhance the performance and accuracy of the predictive model.<br />

### Feature Engineering
New features such as dayOfWeek and hourOfDay were extracted to capture potential patterns in flight prices. Categorical columns, including startingAirport, destinationAirport, isBasicEconomy, isNonStop, and segmentsAirlineName, were indexed and one-hot-encoded. Numeric columns were scaled using MinMaxScaler to ensure uniformity and prevent bias in the model.

![image](https://github.com/user-attachments/assets/c9c98204-fb56-4ff9-8a45-aec9252d4bf0)

![image](https://github.com/user-attachments/assets/2ace2f51-99a4-4d11-903e-1bda32613319)

### Model Development and Validation
A linear regression model was chosen due to the observed linear relationships in the data. The dataset was split into training (80%) and testing (20%) sets. Cross-validation and hyperparameter tuning were employed to optimize the model parameters, ensuring the best performance and minimizing overfitting.
The model's performance was evaluated using Root Mean Squared Error (RMSE). The final RMSE was approximately 1.25, indicating a well-performing model. The error margin for predicted prices was about $1-$2, demonstrating the model's accuracy in forecasting flight prices based on the provided features.

### Visualizations
Various plots were created to illustrate the relationships between actual and predicted prices, error distributions, and the correlation between features. <br />
Key visualizations included:<br />
Scatter plots of actual vs. predicted prices.<br />
Histograms showing the distribution of prediction errors.<br />
Heatmaps displaying correlations between different features.<br />
Time series plots comparing actual and predicted prices over time.<br />

![image](https://github.com/user-attachments/assets/e7ae9542-f097-4d66-b9b4-141961c6dd22)

## Conclusion
The linear regression model effectively predicts flight prices with high accuracy and reliability. Understanding the factors influencing flight prices can help companies optimize pricing and enhance profitability while providing consumer satisfaction.
