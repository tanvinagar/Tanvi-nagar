# Tanvi-nagar
Rainfall Prediction Project — Project Summary
Objective
This project focuses on building a machine learning model to estimate rainfall (precipitation) using daily weather data from Austin, Texas. The aim is to understand how various weather elements—such as temperature, humidity, and wind speed—affect precipitation, and to use that understanding for accurate rainfall prediction.

Methodology
1. Data Import
Loaded the dataset austin_weather.csv using pandas.
Converted the date column to a proper datetime format for time-based analysis.
2. Data Cleaning
Removed non-informative or irrelevant columns like "Events" and "SeaLevelPressureLowInche".
Replaced symbols like "T" (trace rainfall) and "-" with 0.0 to make the data numerically valid.
Converted all applicable fields to numeric format and handled missing values using median imputation.
3. Feature Engineering
Extracted new variables like month and day_of_year from the date to capture seasonality.
Optional: Created lag features for precipitation to include short-term history in the model.
4. Model Training
Applied Linear Regression using scikit-learn to predict the PrecipitationSumInches.
Split the data into training and testing sets for fair evaluation.
5. Model Evaluation
Measured performance using R² (coefficient of determination), Mean Absolute Error (MAE), and Root Mean Squared Error (RMSE).
Compared model predictions with actual values to assess fit and reliability.
6. Visualization
Created time-based plots to show trends in rainfall.
Built scatterplots and regression lines to visualize relationships between rainfall and other variables.
Checked residuals to examine model errors and consistency.

Analysis Steps in Notebook
Setup & Imports – Imported required Python libraries.
Dataset Overview – Displayed first few rows and checked column types.
Cleaning Process – Cleaned and converted data to usable formats.
Exploratory Analysis – Looked at statistical patterns and correlations.
Modeling – Built and tested a Linear Regression model.
Visualization – Plotted trends, predictions, and model behavior.
Interpretation – Reviewed model outputs and drew practical conclusions.

Key Takeaways
Humidity had a positive correlation with rainfall—higher humidity often led to increased precipitation.
Temperature showed an inverse relationship, where hotter days typically saw less rainfall.
Model Accuracy: The Linear Regression model achieved decent performance, with an R² of approximately 0.6 (actual value may vary).
Limitations: Rainfall prediction is inherently noisy; performance could be improved using more complex models like Decision Trees or Random Forests.

Final Thoughts
The project successfully demonstrated how linear models can be used for rainfall prediction based on weather indicators. Although the predictions are not perfect, they provide valuable insight into weather trends. Future improvements could include trying non-linear models, adding more weather-related features, or using deep learning for time-series forecasting.  
