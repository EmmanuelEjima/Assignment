# 🛒 Supermarket Sales Prediction

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/EmmanuelEjima/Data-Science-Machine-Learning-Portfolio/blob/main/projects/Supermarket-Sales-Prediction/Supermarket_Sales_Prediction.ipynb)

## 📋 Project Overview

This project develops a comprehensive **machine learning regression model** to predict supermarket sales using historical transaction data. By analyzing customer demographics, product categories, and shopping patterns, the model enables data-driven decision-making for inventory management, staffing optimization, and revenue forecasting.

This is an end-to-end machine learning project demonstrating:

- Data exploration and preprocessing
- Feature engineering and selection
- Regression model development
- Model evaluation and comparison
- Business insights generation
- Production-ready predictions

---

## 🎯 Objective

The primary goals of this project are to:

✅ **Predict total sales per transaction** with high accuracy  
✅ **Identify key factors** affecting sales performance  
✅ **Analyze customer demographics** and purchasing patterns  
✅ **Generate actionable business insights** for decision-making  
✅ **Optimize inventory management** based on sales predictions  
✅ **Support revenue forecasting** and financial planning  

---

## 📊 Dataset Overview

### Dataset Characteristics:

- **Total Records**: 440 transactions
- **Total Features**: 17 variables
- **Data Sources**: Supermarket chain transaction data
- **Target Variable**: Sales (continuous value in currency)
- **Time Period**: Historical transaction records

### Key Features:

| Feature | Type | Description |
|---------|------|-------------|
| `Invoice ID` | String | Unique transaction identifier |
| `Branch` | Categorical | Supermarket branch location |
| `City` | Categorical | City where branch is located |
| `Customer Type` | Categorical | Member or Normal customer |
| `Gender` | Categorical | Customer gender (Male/Female) |
| `Product Line` | Categorical | Category of product purchased |
| `Unit Price` | Numeric | Price per unit |
| `Quantity` | Numeric | Number of items purchased |
| `Tax` | Numeric | Tax amount on purchase |
| `Total` | Numeric | Total transaction value (TARGET) |
| `Date` | Date | Transaction date |
| `Time` | Time | Transaction time |
| `Payment` | Categorical | Payment method |
| `COGS` | Numeric | Cost of goods sold |
| `Gross Margin` | Numeric | Gross profit margin |
| `Rating` | Numeric | Customer satisfaction rating (1-10) |

---

## 🔍 Key Insights & Findings

### Sales Drivers:

**1. Quantity Purchased** - Strongest predictor of sales
   - Direct linear relationship with total sales
   - Bulk purchases significantly increase transaction value

**2. Unit Price Impact** - Premium products generate higher sales
   - Higher-priced items contribute more to revenue
   - Strong correlation with transaction totals

**3. Product Line Variation** - Different categories perform differently
   - Electronics and Home & Lifestyle have higher average sales
   - Fashion and Sports products show lower average values

**4. Customer Type Differences** - Members vs Normal customers
   - Member purchases may show different patterns
   - Loyalty impacts transaction value

**5. Payment Method Influence** - Multiple payment options available
   - Different payment methods may correlate with spending
   - Customer preference affects purchase decisions

**6. Customer Satisfaction** - Rating correlates with sales
   - Higher satisfaction ratings on larger purchases
   - Customer experience impacts loyalty and sales

### Business Intelligence:

- **Peak Sales Times**: Certain time periods show higher transactions
- **Branch Performance**: Different locations have varying sales patterns
- **City Insights**: Geographic location influences purchasing behavior
- **Gender Preferences**: Different product line preferences by gender
- **Seasonal Patterns**: Sales fluctuate based on shopping periods

---

## 🤖 Machine Learning Approach

### Data Preprocessing:

✅ **Data Cleaning**
   - Handled missing values
   - Removed duplicates
   - Validated data types

✅ **Feature Engineering**
   - Created derived features from raw data
   - Encoded categorical variables (One-Hot Encoding)
   - Normalized and scaled numerical features

✅ **Exploratory Data Analysis**
   - Analyzed feature distributions
   - Computed correlation matrices
   - Identified outliers and anomalies

### Regression Models Implemented:

1. **Linear Regression**
   - Baseline model for comparison
   - Simple and interpretable
   
2. **Decision Tree Regression**
   - Captures non-linear relationships
   - Feature importance visualization
   
3. **Random Forest Regression**
   - Ensemble method for improved accuracy
   - Reduces overfitting
   - Provides robust predictions

4. **Gradient Boosting Regression** (if applicable)
   - Advanced ensemble technique
   - Optimal for complex patterns

### Model Evaluation Metrics:

| Metric | Description | Target |
|--------|-------------|--------|
| **R² Score** | Coefficient of determination (0-1) | Closer to 1 = Better |
| **Mean Absolute Error (MAE)** | Average absolute prediction error | Lower = Better |
| **Root Mean Squared Error (RMSE)** | Penalizes larger errors more | Lower = Better |
| **Mean Squared Error (MSE)** | Average of squared errors | Lower = Better |

---

## 📈 Model Performance Results

### Best Performing Model: [Model Name]

| Metric | Training Set | Testing Set |
|--------|--------------|------------|
| **R² Score** | [Value] | [Value] |
| **MAE** | $[Value] | $[Value] |
| **RMSE** | $[Value] | $[Value] |
| **MSE** | $[Value] | $[Value] |

### Model Comparison:

| Algorithm | R² Score | MAE | RMSE |
|-----------|----------|-----|------|
| Linear Regression | [Value] | [Value] | [Value] |
| Decision Tree | [Value] | [Value] | [Value] |
| Random Forest | [Value] | [Value] | [Value] |
| Gradient Boosting | [Value] | [Value] | [Value] |

---

## 🛠️ Technologies & Libraries

- **Python 3.8+** - Programming language
- **Pandas** - Data manipulation and analysis
- **NumPy** - Numerical computations
- **Matplotlib** - Visualization library
- **Seaborn** - Statistical data visualization
- **Scikit-learn** - Machine learning algorithms
- **Jupyter** - Interactive notebook environment
- **Google Colab** - Cloud-based execution

---

## 📂 Project Structure

```text
Supermarket-Sales-Prediction/
│
├── Supermarket_Sales_Prediction.ipynb    # Main analysis & modeling notebook
├── README.md                              # Project documentation
└── images/
    └── (Visualization outputs and charts)
```

---

## ▶️ Run the Analysis

### Option 1: Google Colab (Recommended - No Setup Required)

Click the **"Open in Colab"** badge at the top of this README to run the analysis directly in your browser.

### Option 2: Run Locally

#### Clone the repository

```bash
git clone https://github.com/EmmanuelEjima/Data-Science-Machine-Learning-Portfolio.git
```

#### Navigate to the project folder

```bash
cd projects/Supermarket-Sales-Prediction
```

#### Install dependencies

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

#### Or install from requirements (if available)

```bash
pip install -r requirements.txt
```

#### Launch Jupyter Notebook

```bash
jupyter notebook Supermarket_Sales_Prediction.ipynb
```

The notebook will open in your default browser at `http://localhost:8888`

---

## 📓 Notebook Contents

The **Supermarket_Sales_Prediction.ipynb** notebook includes:

1. **Data Loading** - Import and initial inspection
2. **Exploratory Data Analysis (EDA)** - Dataset overview and statistics
3. **Data Cleaning** - Handling missing values and outliers
4. **Feature Engineering** - Creating new features and encoding
5. **Correlation Analysis** - Identifying feature relationships
6. **Data Visualization** - Charts and plots for insights
7. **Feature Scaling** - Normalization and standardization
8. **Train-Test Split** - Preparing data for modeling
9. **Model Development** - Training multiple regression models
10. **Model Evaluation** - Comparing performance metrics
11. **Hyperparameter Tuning** - Optimizing best performing model
12. **Feature Importance** - Identifying key predictors
13. **Predictions** - Making sales forecasts
14. **Summary & Conclusions** - Key findings and recommendations

---

## 💡 Key Features of Analysis

### 1. Comprehensive EDA
- Univariate analysis of each feature
- Bivariate relationships with target variable
- Multivariate correlation analysis
- Distribution and outlier detection

### 2. Feature Engineering
- Derived features from temporal data
- Categorical encoding strategies
- Feature scaling techniques
- Dimensionality consideration

### 3. Regression Modeling
- Multiple algorithm comparison
- Cross-validation for robust evaluation
- Hyperparameter optimization
- Overfitting prevention

### 4. Business Intelligence
- Sales pattern identification
- Product line performance
- Customer segmentation insights
- Revenue optimization recommendations

---

## 🎯 Business Recommendations

Based on the analysis and model insights:

1. **Inventory Optimization**
   - Stock popular product lines with higher sales predictions
   - Adjust inventory levels based on seasonal patterns
   - Focus on high-margin products

2. **Staffing & Operations**
   - Allocate more staff during predicted peak sales periods
   - Optimize checkout counters based on transaction volume
   - Enhance customer service during high-traffic times

3. **Marketing Strategy**
   - Target promotions on high-performing product lines
   - Develop loyalty programs for member customers
   - Create bundle deals with complementary products

4. **Pricing Strategy**
   - Analyze unit price impact on sales
   - Implement dynamic pricing for optimal revenue
   - Consider competitor pricing strategies

5. **Customer Experience**
   - Monitor and improve ratings for repeat business
   - Personalize recommendations based on purchase history
   - Enhance shopping experience for different customer types

---

## 📌 Future Enhancements

- Time series forecasting for trend prediction
- Customer segmentation and clustering analysis
- Recommendation system for product bundling
- Real-time sales prediction dashboard
- Advanced ensemble methods (XGBoost, LightGBM)
- Deep learning models (Neural Networks)
- A/B testing framework for marketing experiments
- Interactive Streamlit dashboard for business stakeholders

---

## ⚠️ Disclaimer

This analysis is for **educational and portfolio purposes only**. While the models provide predictive insights, real-world business decisions should be made by incorporating domain expertise, market conditions, and additional factors not captured in this dataset.

---

## 📚 Dataset Source

The supermarket sales dataset used in this analysis is:
- A publicly available retail transaction dataset
- Commonly used for machine learning education
- Contains realistic customer transaction patterns
- Suitable for regression modeling practice

---

## 👨‍💻 Author

**Emmanuel Ejima**

Chemical Engineer | Data Science & Machine Learning Enthusiast | Renewable Energy Engineer

- **GitHub:** https://github.com/EmmanuelEjima
- **LinkedIn:** https://linkedin.com/in/emmanuel-ejima
- **Portfolio:** https://github.com/EmmanuelEjima/Data-Science-Machine-Learning-Portfolio

---

⭐ **If you found this project useful, consider giving it a Star on GitHub!**
