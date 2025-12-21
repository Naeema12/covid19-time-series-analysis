# COVID-19 Time Series Forecasting

This project focuses on the time series analysis and forecasting of daily COVID-19 cases in Turkey.  
Classical statistical models and deep learning approaches are compared to evaluate their performance on real-world pandemic data.

## Dataset
The dataset contains daily COVID-19 statistics reported in Turkey, including daily case numbers, tests, deaths, and recoveries.  
In this study, the daily number of confirmed cases is used as the main time series variable.

## Data Preprocessing
Several preprocessing steps were applied before modeling:
- Handling missing values
- Detecting and cleaning extreme spike values
- Calculating 7-day moving averages for trend analysis
- Time series decomposition into trend, seasonal, and residual components
- Normalization of data for LSTM model using Min-Max scaling

These steps help improve model stability and forecasting accuracy.

## Models Used
The following models were implemented and compared:
- **ARIMA**: Classical time series model for trend-based forecasting
- **SARIMAX**: Seasonal ARIMA model considering temporal patterns
- **LSTM**: Deep learning model capable of learning complex and non-linear temporal dependencies

## Evaluation Metric
Model performance was evaluated using:
- **RMSE (Root Mean Squared Error)**

RMSE values were calculated by comparing predicted values with actual test data.

## Results
The results show that:
- ARIMA and SARIMAX models can capture the general trend of the time series
- LSTM model performs better in capturing sudden changes and complex patterns
- LSTM achieved the lowest RMSE value among the tested models

The findings are consistent with similar studies in the literature.

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Statsmodels
- TensorFlow / Keras

## Conclusion
This project demonstrates the effectiveness of combining classical time series models and deep learning approaches for pandemic data forecasting.  
The comparative analysis highlights the strengths and limitations of each method.


