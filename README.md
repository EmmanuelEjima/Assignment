# Supermarket Sales Prediction

This project builds a machine learning model to predict total sales per transaction using a public supermarket sales dataset. The goal is to support better inventory management, staffing decisions, and overall business strategy.

## Dataset
The dataset contains 1,000 supermarket transactions with customer, product, pricing, and payment information. It includes both categorical and numerical features.

## Methodology
- Data cleaning and preprocessing
- Exploratory data analysis (EDA)
- Feature engineering and encoding
- Regression modeling (Linear Regression, Decision Tree, Random Forest)
- Model evaluation using MAE, RMSE, and R² score

## Results
After removing features that caused data leakage, tree-based models significantly outperformed linear regression. The Random Forest Regressor achieved the best performance with the highest R² score and lowest error metrics.

## Tools Used
- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn
- Google Colab

## Business Insights
The model highlights the importance of product type, unit price, quantity purchased, and customer behavior in driving sales. These insights can help supermarkets improve demand forecasting and operational planning.
