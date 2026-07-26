# 🚢 Titanic Survival Analysis

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/EmmanuelEjima/Data-Science-Machine-Learning-Portfolio/blob/main/projects/Titanic-Survival-EDA/Titanic_Survival_EDA_Analysis.ipynb)

## 📋 Project Overview

This project performs a comprehensive **Exploratory Data Analysis (EDA)** on the Titanic dataset to identify and analyze the key factors that influenced passenger survival during the tragic 1912 disaster. Through detailed statistical analysis and data visualization, this project uncovers patterns in passenger demographics, ticket pricing, and embarking ports that affected survival rates.

This is a classic data science project demonstrating:

- Data cleaning and preprocessing
- Exploratory Data Analysis (EDA) best practices
- Statistical analysis
- Data visualization techniques
- Pattern identification and insights
- Reproducible analysis workflows

---

## 📌 Objective

Perform comprehensive Exploratory Data Analysis (EDA) on the Titanic dataset to:

✅ Identify factors affecting passenger survival  
✅ Analyze demographic patterns (age, gender, class)  
✅ Examine ticket pricing and passenger class relationships  
✅ Discover embarking port influences  
✅ Uncover correlations between variables  
✅ Generate actionable insights from historical data

---

## 📊 Dataset Overview

### Dataset Characteristics:

- **Total Records**: 891 passengers
- **Survived**: 342 passengers (38.4%)
- **Did Not Survive**: 549 passengers (61.6%)
- **Features**: 12 columns including passenger metadata and survival status

### Key Variables:

| Variable | Type | Description |
|----------|------|-------------|
| `PassengerId` | Numeric | Unique passenger identifier |
| `Survived` | Binary | Survival status (0 = No, 1 = Yes) |
| `Pclass` | Numeric | Ticket class (1 = 1st, 2 = 2nd, 3 = 3rd) |
| `Name` | String | Passenger name |
| `Sex` | Categorical | Passenger gender (Male/Female) |
| `Age` | Numeric | Passenger age in years |
| `SibSp` | Numeric | Number of siblings/spouses aboard |
| `Parch` | Numeric | Number of parents/children aboard |
| `Ticket` | String | Ticket number |
| `Fare` | Numeric | Ticket price (in pounds) |
| `Cabin` | String | Cabin number |
| `Embarked` | Categorical | Port of embarkation (C/Q/S) |

---

## 🔍 Key Findings & Insights

### Gender Impact (Most Significant Factor):
- **Female Survival Rate**: 74.2% - Nearly 3x higher than males
- **Male Survival Rate**: 18.9% - Reflects "Women and Children First" policy
- Gender is the strongest predictor of survival

### Ticket Class Distribution:
- **1st Class Survival**: 63.0% - Best survival chances
- **2nd Class Survival**: 47.3% - Moderate survival rate
- **3rd Class Survival**: 24.2% - Lowest survival rate
- Clear socioeconomic advantage in survival

### Age Patterns:
- **Children (Age < 5)**: Highest survival rate (~96%)
- **Young Adults (Age 20-40)**: Moderate survival
- **Elderly Passengers (Age > 60)**: Lower survival rates
- Age inversely correlates with survival

### Family Size Impact:
- Passengers traveling alone had lower survival rates
- Families of 2-3 members had better survival outcomes
- Large families (5+ members) had difficulty evacuating together

### Embarkation Port Analysis:
- **Cherbourg (C)**: Highest average fare - 1st class passengers
- **Southampton (S)**: Mixed class distribution
- **Queenstown (Q)**: Predominantly 3rd class passengers

### Fare Analysis:
- Strong correlation between ticket price and survival
- Higher fare passengers had better access to lifeboats
- Average fare for survivors: £51.86
- Average fare for non-survivors: £22.11

---

## 📈 Analysis Methodology

### Data Cleaning:
- Handled missing values (Age, Cabin, Embarked)
- Removed irrelevant columns (PassengerId, Ticket)
- Standardized data types and formats

### Exploratory Analysis:
1. **Univariate Analysis**: Distribution of individual variables
   - Survival count and percentage
   - Age distribution
   - Fare distribution
   - Class distribution

2. **Bivariate Analysis**: Relationships between two variables
   - Survival vs Gender
   - Survival vs Ticket Class
   - Survival vs Age
   - Survival vs Fare
   - Survival vs Port of Embarkation

3. **Multivariate Analysis**: Complex relationships
   - Gender + Class interaction
   - Age + Class patterns
   - Family size + Survival correlation

### Visualization Techniques:
- Count plots for categorical distributions
- Histograms for numerical distributions
- Box plots for outlier detection
- Heatmaps for correlation analysis
- Cross-tabulations for categorical relationships
- Violin plots for distribution comparisons

---

## 🛠️ Technologies & Libraries

- **Python 3.8+** - Programming language
- **Pandas** - Data manipulation and analysis
- **NumPy** - Numerical computations
- **Matplotlib** - Visualization library
- **Seaborn** - Statistical data visualization
- **Jupyter** - Interactive notebook environment
- **Google Colab** - Cloud-based execution

---

## 📂 Project Structure

```text
Titanic-Survival-EDA/
│
├── Titanic_Survival_EDA_Analysis.ipynb    # Main analysis notebook
├── README.md                               # Project documentation
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
cd projects/Titanic-Survival-EDA
```

#### Install dependencies

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

#### Or install from requirements (if available)

```bash
pip install -r requirements.txt
```

#### Launch Jupyter Notebook

```bash
jupyter notebook Titanic_Survival_EDA_Analysis.ipynb
```

The notebook will open in your default browser at `http://localhost:8888`

---

## 📓 Notebook Contents

The **Titanic_Survival_EDA_Analysis.ipynb** notebook includes:

1. **Data Loading** - Import and initial inspection
2. **Data Overview** - Dataset shape, info, and statistics
3. **Missing Values Analysis** - Identify and visualize missing data
4. **Survival Distribution** - Overall survival statistics
5. **Gender Analysis** - Impact on survival rates
6. **Class Analysis** - Ticket class and survival correlation
7. **Age Analysis** - Age group survival patterns
8. **Fare Analysis** - Ticket price and survival relationship
9. **Family Size Analysis** - Impact of traveling with family
10. **Port Analysis** - Embarkation port patterns
11. **Correlation Analysis** - Heatmap of all variables
12. **Summary of Findings** - Key insights and conclusions

---

## 💡 Key Insights Summary

### The "Women and Children First" Policy:
- Clear evidence of prioritizing female and young passengers
- Resulted in a 3x survival rate difference between genders

### Class Privilege:
- 1st class passengers were almost 3x more likely to survive
- Access to lifeboats was strongly correlated with ticket class
- Socioeconomic status was a critical survival factor

### Age Advantage:
- Children had the highest survival chances
- Working-age adults had moderate survival rates
- Elderly passengers faced lower survival probabilities

### Family Dynamics:
- Traveling with family provided better survival chances
- Parents prioritized children's safety
- Separated families had worse outcomes

### Economic Disparity:
- Ticket fare was a strong proxy for survival chances
- Premium passengers had better lifeboat access
- Economic class was a major survival determinant

---

## 🎯 Learning Outcomes

By studying this analysis, you'll learn:

✅ How to perform comprehensive EDA  
✅ Data cleaning and preprocessing techniques  
✅ Statistical analysis methods  
✅ Data visualization best practices  
✅ Pattern recognition in historical datasets  
✅ How to communicate findings effectively  
✅ Exploratory data analysis workflow

---

## 📌 Future Enhancements

- Interactive visualizations with Plotly
- Predictive modeling (predict survival probability)
- Machine learning classification models
- Dashboard creation with Streamlit
- Statistical hypothesis testing
- Advanced correlation analysis (Cramer's V, Spearman correlation)
- Time-based analysis (if temporal data available)

---

## ⚠️ Disclaimer

This analysis is for **educational and portfolio purposes only**. While the Titanic dataset is historical and widely used in data science education, the insights should be understood within their historical context and not used to make real-world predictions about modern scenarios.

---

## 📚 Dataset Source

The Titanic dataset used in this analysis is:
- Widely available through Kaggle and other data repositories
- A classic dataset used extensively in data science education
- Based on historical records from the RMS Titanic disaster (April 15, 1912)
- Contains real passenger information from the tragedy

---

## 👨‍💻 Author

**Emmanuel Ejima**

Chemical Engineer | Data Science & Machine Learning Enthusiast | Renewable Energy Engineer

- **GitHub:** https://github.com/EmmanuelEjima
- **LinkedIn:** https://linkedin.com/in/emmanuel-ejima
- **Portfolio:** https://github.com/EmmanuelEjima/Data-Science-Machine-Learning-Portfolio

---

⭐ **If you found this analysis useful, consider giving it a Star on GitHub!**
