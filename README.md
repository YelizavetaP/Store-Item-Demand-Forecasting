# Store-Item-Demand-Forecasting

## 1. Statement of the Problem
The primary task is to accurately forecast the demand for store items to optimize inventory management. This involves predicting future sales based on historical sales data.

## 2. Sources and Description of Data
The dataset used for this project is sourced from [Store Item Demand Forecasting Challenge](https://www.kaggle.com/competitions/demand-forecasting-kernels-only/overview), which includes historical sales data for various store items over 5 years.

- **Data Structure**: 
- `date`: The date of the sales record.
- `store_id`: The identifier for the store.
- `item_id`: The identifier for the product.
- `sales`: The number of items sold on that date.
  
## 3. Approach to the Solution
To solve the problem, the following methodology and tools were employed:

- **Feature Engineering**: Additional features such as hour, day of the week, quarter, year, and sine/cosine transformations of the day of the year were created to capture seasonal patterns.
- **Machine Learning Models**: Several models were tested, including `Naive model`, `XGBModel`, `ExponentialSmoothing`, `ARIMA`, `AutoARIMA`, `Prophet` and `RNN` model to find the best-performing model for demand forecasting.
`Backtesting` was conducted to evaluate the performance of thrthe best model by comparing predictions against actual historical sales data.
- **Tools and Libraries**: The project utilized Python with libraries such as `Pandas` for data manipulation, `NumPy` for numerical operations, `Scikit-learn` and `statsmodels` for implementing ML algorithms, `Darts` for time series handling, and `Matplotlib/Seaborn` for data visualization.

## 4. Obtained Results and Conclusions
The analysis revealed that the demand forecasting model achieved a high level of accuracy with `MAPE score 20.9%` on `Prophet` model. The model effectively captured the seasonal trends and patterns in the sales data, allowing for reliable demand predictions.


### Findings and Suggestions for Improvement
- **Exploration of Advanced Techniques**: Testing more sophisticated algorithms, such as XGBoost or LSTM, could lead to further improvements in predictive performance.
- **Scalability**: Expand the model to include additional items and stores for a more comprehensive forecasting solution.
- **Visualization**: Develop a dashboard  to easily visualize forecasts

By addressing these areas, the project can evolve into a robust demand forecasting solution that significantly enhances the operational efficiency and strategic planning of the store.