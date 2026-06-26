Store Sales Forecasting using Machine Learning

Project Overview

This project aims to predict retail store sales using Machine Learning. Accurate sales forecasting helps businesses make informed decisions about inventory management, staffing, promotions, and demand planning.

A Random Forest Regressor was trained using historical sales data along with information about holidays, promotions, store details, customer transactions, and oil prices. A time-based train-test split was used to simulate real-world forecasting, ensuring that future sales were predicted using only past data.


Objectives

- Forecast future store sales using historical data.
- Analyze how promotions affect sales.
- Study the impact of holidays on customer purchasing behavior.
- Evaluate the influence of customer transactions and oil prices.
- Build a robust Machine Learning model for sales prediction.


Dataset

The project uses the Store Sales - Time Series Forecasting dataset from Kaggle.

The following datasets were used:

- train.csv
- stores.csv
- holidays_events.csv
- transactions.csv
- oil.csv

> Note: The dataset is not included in this repository because of its size. It can be downloaded directly from Kaggle.

Technologies Used

 Technology                       Purpose 

 Python                     | Programming Language 
 Pandas                     | Data Manipulation 
 NumPy                      | Numerical Computing 
 Matplotlib                 | Data Visualization 
 Scikit-learn               | Machine Learning 
 Jupyter Notebook           | Development Environment 



 Project Workflow

1. Data Collection
2. Data Cleaning
3. Merge Multiple Datasets
4. Feature Engineering
5. Handle Missing Values
6. Encode Categorical Variables
7. Time-Based Train-Test Split
8. Train Random Forest Regression Model
9. Evaluate Model Performance
10. Analyze Feature Importance
11. Generate Business Insights


Machine Learning Model

Algorithm Used

- Random Forest Regressor

Reason for Choosing

Random Forest is capable of handling nonlinear relationships, works well with tabular data, reduces overfitting through ensemble learning, and provides feature importance scores that help interpret the model.


 Model Performance

  Metric    Value 

  MAE       125.59 
  RMSE      393.87 
  R² Score  0.9184 

The model achieved an R² score of 91.84%, indicating excellent predictive performance on unseen future data.



 Top Features Influencing Sales

Based on the trained Random Forest model:

 Feature          Importance 

 Product Family   41.6% 
 Transactions     24.5% 
 On Promotion     20.6% 
 Store Cluster     1.4% 
 Store Number      1.3%  
 Oil Price         1.0% 


 Business Insights

- Product category has the strongest influence on sales.
- Promotional campaigns significantly increase customer purchases.
- Higher customer transactions generally result in higher sales.
- Holidays contribute to seasonal variations in demand.
- Oil prices have only a small impact on sales compared to promotions and customer traffic.



 Project Structure


sales_data_forecasting_project/
│
├── data/
├── notebook/
│   └── Store_Sales_Forecasting.ipynb
│
├── images/
├── README.md
├── requirements.txt
└── .gitignore



 Future Improvements

- Experiment with XGBoost and LightGBM.
- Perform hyperparameter tuning.
- Build an interactive Streamlit dashboard.
- Deploy the model as a web application.
- Incorporate additional external features such as weather data.

