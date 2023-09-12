# timeseries-fb-prophet
time series analysis and forecasting on energy consumption data using the Prophet library
The readme file on this project was generated using gpt as the llms are excellent at generating textual daat. chatgpt can explain the project better than me i suppose

1. It imports necessary libraries, including NumPy, pandas, seaborn, and Prophet, and sets some plotting styles.

2. Defines a function `mean_absolute_percentage_error` to calculate a common error metric for forecasting accuracy.

3. Reads a time series dataset from a CSV file named 'PJME_hourly.csv' into a pandas DataFrame called `pjme`.

4. Plots the time series data to visualize the energy consumption over time.

5. Defines a function `create_features` to extract various time-related features from the datetime index of the dataset, such as hour, day of the week, quarter, month, etc.

6. Applies the `create_features` function to the `pjme` dataset, creating a new DataFrame `features_and_target` with both features and the target variable.

7. Plots a boxplot to visualize the energy consumption by day of the week and season.

8. Splits the dataset into training and test sets based on a split date, '1-Jan-2015', and visualizes the split.

9. Prepares the training dataset for Prophet by renaming columns and setting the 'ds' (datetime) and 'y' (target) columns.

10. Initializes and fits a Prophet model to the training data.

11. Prepares the test dataset for Prophet in a similar manner.

12. Uses the trained Prophet model to make predictions on the test dataset.

13. Visualizes the forecasted values compared to the actual values for a specific date range.

14. Evaluates the model's performance using various error metrics, such as RMSE, MAE, and MAPE.

15. Adds holidays to the Prophet model by creating a holiday dataframe and fitting a new model with holidays included.

16. Makes predictions with the model that includes holidays.

17. Visualizes components of the forecasted data, such as trends and holidays.

18. Makes predictions for future data points using the trained model.

Overall, this code demonstrates how to load time series data, preprocess it, use the Prophet library for forecasting, evaluate the model's performance, and make future predictions.
