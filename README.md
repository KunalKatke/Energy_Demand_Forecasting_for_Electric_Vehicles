# Energy Demand Forecasting for Electric Vehicles

## Introduction
The transition to electric vehicles (EVs) is accelerating globally, necessitating accurate forecasting of energy demand to ensure the reliability of power supply systems. This project aims to develop effective forecasting models that predict energy consumption based on historical electricity data delivered for EV charging. Accurate forecasting is essential for optimizing grid operations, reducing costs, and planning infrastructure development.

## Objectives
- Implement the Prophet forecasting model to generate accurate forecasts based on historical energy consumption data.
- Apply traditional machine learning and statistical models (Random Forest, Linear Regression, KNN, ARIMA) to evaluate their effectiveness in capturing patterns in time series data.
- Compare the performance of different machine learning models with ARIMA and Prophet results.

## Dataset Description
The dataset used in this project was downloaded from the ACN-Data portal and includes detailed information about each EV charging session. Key columns include:
- **Date:** The date of the charging sessions.
- **number_of_devices:** The count of devices charged on that date.
- **total_kWh_delivered:** The total kilowatt-hours delivered during the sessions.

## Methodology
1. **Data Preprocessing:**
   - Handling missing values using interpolation.
   - Outlier detection using the z-score method.
   - Dropping unnecessary columns.

2. **Stationarity Testing:**
   - Conducting Augmented Dickey-Fuller (ADF) and KPSS tests to check for stationarity.

3. **Feature Engineering:**
   - Creating lag features and calculating rolling statistics.

4. **Data Splitting:**
   - Dividing the dataset into training, testing, and validation sets.

5. **Modeling:**
   - Implementing five models: Random Forest, Linear Regression, KNN, ARIMA, and Prophet.
   - Using Python libraries such as Scikit-learn, Statsmodels, and Facebook's Prophet.

## Results
The models were evaluated based on MAE, RMSE, and MSE metrics. Notably:
- **Linear Regression** achieved the lowest RMSE of 47.93.
- **Random Forest** followed with an RMSE of 53.87.
- Both **ARIMA** and **Prophet** performed less effectively compared to the machine learning models.

## Conclusion
This project successfully demonstrated the effectiveness of various forecasting models in predicting energy demand for electric vehicles based on historical charging data. The findings suggest that machine learning approaches may be better suited for modeling complex relationships in time series data associated with EV energy consumption.

## Future Work
Future explorations could include:
- Hyperparameter tuning and ensemble methods.
- Incorporating external factors like weather conditions or socio-economic indicators to improve model robustness.

## Installation
To run this project locally:
1. Clone the repository:
