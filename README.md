Retail-Sales-Prediction-ROSSMANN image

Rossmann operates over 3,000 drug stores in 7 European countries. Currently, Rossmann store managers are tasked with predicting their daily sales for up to six weeks in advance. Store sales are influenced by many factors, including promotions, competition, school and state holidays, seasonality, and locality. With thousands of individual managers predicting sales based on their unique circumstances, the accuracy of results can be quite varied. My work includes various plots and graphs , visualizations , feature engineering , ensemble techniques , different ML algorithms with their respective parameter tuning , analysis and trends . Predictions are of 6 weeks of daily sales for 1,115 stores located across Germany.

The work here forecasts the sales of the various Rossmann stores across Europe for the recent six weeks and compares the results from the models developed with the actual sales values.

The dataset consists of two csv files: rossmann store data.csv and store.csv

Data Files:

store.csv holds info about each store. rossmann store data.csv holds the sales info per day for each store.

1. Business Problem.
Rossmann operates over 3,000 drug stores in 7 European countries. Currently, Rossmann store managers are tasked with predicting their daily sales for up to six weeks in advance. Store sales are influenced by many factors, including promotions, competition, school and state holidays, seasonality, and locality. With thousands of individual managers predicting sales based on their unique circumstances, the accuracy of results can be quite varied.

2. Solution Strategy
My strategy to solve this challenge was:

Step 01: Know Your Data: Use info(),head(),tail(),find missing values and impute them,remove duplicates.

Step 02: Understand Your Variables: find uniqueness, their datatypes, any irregularity among them,describing variables etc.

Step 03: Data Wrangling & Data Visualization: Explore the data to find insights and better understand the impact of variables on model learning.

Step 04: Hypothesis testing: make some hypothesis based on data visualization insights and perform statistical test.

Step 05: Feature Engineering: Selection, manipulation, handling missing & outliers, data transformation on selected features and train-test split of the most significant attributes for training the model.

Step 06: Machine Learning Modelling: Machine Learning model training.

Step 07: Hyperparameter Fine Tunning: hoose the best values for each of the parameters of the model selected from the previous step.

Step 08: Deploy Modelo to Production: Publish the model in a cloud environment so that other people or services can use the results to improve the business decision.

3. Top Data Insights
there were more sales on Monday, probably because shops generally remain closed on Sundays which had the lowest sales in a week. This validates the hypothesis about this feature.
The positive effect of promotion on Customers and Sales is observable.
Most stores have competition distance within the range of 0 to 10 kms and had more sales than stores far away probably indicating competition in busy locations vs remote locations.
Store type B though being few in number had the highest sales average. The reasons include all three kinds of assortments specially assortment level b which is only available at type b stores and being open on sundays as well.
The outliers in the dataset showed justifiable behaviour. The outliers were either of store type b or had promotion going on which increased sales.
4. Machine Learning Model Applied
At this stage, 4 models were used for analysis: *Linear Regression Random Forest Regressor XGBoost RegressorDecision tree

5. Machine Learning Model Performance
Performance of Random Forest Regressor Model:
R-squared (Test): 0.9809 Mean Absolute Error (Test): 297.47 Root Mean Squared Error (Test): 470.09

7. Conclusions
The sales forecast and the generated insights provide the CEO with valuable tools to decide the amount of budget that is going to be dedicated to the restoration of each store.
