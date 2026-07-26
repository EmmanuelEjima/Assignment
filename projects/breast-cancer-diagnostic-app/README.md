# ⚕️ Breast Cancer Diagnostic Assistant

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/EmmanuelEjima/Data-Science-Machine-Learning-Portfolio/blob/main/projects/breast-cancer-diagnostic-app/Breast%20Cancer%20Detection%20Model.ipynb)
[![Streamlit App](https://img.shields.io/badge/Live%20Demo-Streamlit-red?logo=streamlit)](https://breast-cancer-diagnostic-assistant.streamlit.app/)

## 📷 Application Preview

<p align="center">
  <img src="images/app-preview.jpg" alt="Breast Cancer Diagnostic Assistant" width="900">
</p>

An end-to-end Machine Learning web application that predicts whether a breast tumor is **Malignant** or **Benign** using the **Wisconsin Diagnostic Breast Cancer (WDBC)** dataset. The project demonstrates best practices in model development, deployment, and reproducible ML workflows.

## 📌 Project Overview

This project implements a standardized Machine Learning pipeline for breast cancer diagnosis. Users can enter **30 clinical features** extracted from Fine Needle Aspirate (FNA) images of breast masses.

The project demonstrates best practices in:

- Data preprocessing
- Feature engineering
- Model evaluation
- Model serialization
- Web application deployment
- Reproducible machine learning workflows

---

## ✨ Features

- Interactive Streamlit web application
- Complete 30-feature clinical input interface
- Real-time prediction (Malignant or Benign)
- Confidence score for predictions
- Logistic Regression classifier
- StandardScaler preprocessing pipeline
- Serialized model using Joblib
- Production-ready deployment
- Responsive user interface

---

## 📊 Machine Learning Workflow

- Data Loading
- Exploratory Data Analysis (EDA)
- Data Preprocessing
- Feature Scaling using StandardScaler
- Model Training
- Cross Validation
- Model Evaluation
- Model Serialization (`.pkl`)
- Streamlit Deployment

---

## 📈 Model Performance

| Metric | Value |
|---------|-------|
| **Algorithm** | Logistic Regression |
| **Dataset** | Wisconsin Diagnostic Breast Cancer (WDBC) |
| **Cross-Validation Accuracy** | **≈98.1%** |
| **Framework** | Scikit-learn |
| **Training Samples** | 569 |
| **Features** | 30 |

### Detailed Metrics

- **Precision**: High specificity for malignant classification
- **Recall**: Excellent sensitivity for detecting malignant cases
- **F1-Score**: Well-balanced performance across both classes

---

## 🛠️ Technologies Used

- Python 3.8+
- Streamlit
- Scikit-learn
- Pandas
- NumPy
- Joblib
- Google Colab
- Git
- GitHub

---

## 📂 Project Structure

```text
breast-cancer-diagnostic-app/
│
├── Breast Cancer Detection Model.ipynb    # Full model development & EDA
├── app.py                                  # Streamlit web application
├── README.md                               # Project documentation
├── requirements.txt                        # Python dependencies
├── models/
│   ├── breast_cancer_model.pkl            # Trained Logistic Regression model
│   └── scaler.pkl                         # StandardScaler for feature normalization
└── images/
    └── app-preview.jpg                    # Application screenshot
```

---

## ▶️ Run the Project Locally

### Clone the repository

```bash
git clone https://github.com/EmmanuelEjima/Data-Science-Machine-Learning-Portfolio.git
```

### Navigate to the project folder

```bash
cd projects/breast-cancer-diagnostic-app
```

### Install dependencies

```bash
pip install -r requirements.txt
```

### Launch the application

```bash
streamlit run app.py
```

The application will open in your default browser at `http://localhost:8501`

---

## 📚 Dataset

The model was trained using the **Wisconsin Diagnostic Breast Cancer (WDBC)** dataset available through Scikit-learn.

### Dataset Characteristics:

- **Sample Size**: 569 observations
- **Features**: 30 numerical features computed from digitized FNA images
- **Classes**: 2 (Malignant or Benign)

Each observation is classified as either:

- 🔴 **Malignant (Cancerous)** - Class: 0
- 🟢 **Benign (Non-cancerous)** - Class: 1

### Feature Categories:

1. **Mean Features** (10): radius, texture, perimeter, area, smoothness, compactness, concavity, concave points, symmetry, fractal dimension
2. **Standard Error Features** (10): Same measurements as above (error values)
3. **Worst Features** (10): Largest values for each measurement type

---

## 💡 How to Interpret Results

### Prediction Output:

- **Malignant (🚨)**: Model detected feature patterns commonly associated with cancerous tumors
- **Benign (✅)**: Model detected feature patterns consistent with non-cancerous tumors

### Confidence Score:

- Ranges from **0% to 100%**
- Higher confidence indicates stronger pattern match
- Example: 95% confidence means the model is 95% certain about the prediction

---

## 📌 Future Improvements

- Enhanced prediction probability visualization
- Interactive visual analytics & feature importance plots
- Comparison with multiple ML algorithms (SVM, Random Forest, Neural Networks)
- Explainable AI integration (SHAP/LIME)
- Docker containerization for easier deployment
- CI/CD deployment pipeline
- Performance metrics dashboard
- Model retraining automation

---

## ⚠️ Disclaimer & Limitations

### Important Disclaimer:

This application is intended for **educational, research, and portfolio purposes only**. It is **not a medical diagnostic system** and should not replace professional medical advice or clinical diagnosis.

### Known Limitations:

1. **Dataset-Specific**: Model trained exclusively on WDBC dataset. Performance may vary on other breast cancer datasets.
2. **Preprocessing Dependencies**: Predictions require exact StandardScaler normalization applied during training.
3. **Model Interpretability**: Logistic Regression provides basic explainability but limited insight into complex feature interactions.
4. **Clinical Validation**: Not clinically validated or FDA-approved.
5. **Use Case**: For demonstration and learning purposes only.

### Proper Use Cases:

- ✅ Learning and understanding ML pipelines
- ✅ Portfolio demonstration
- ✅ Educational research
- ✅ Model development practice

### Not Suitable For:

- ❌ Clinical decision-making
- ❌ Patient diagnosis
- ❌ Medical treatment planning
- ❌ Healthcare deployment without clinical validation

---

## 📓 Jupyter Notebook

The **`Breast Cancer Detection Model.ipynb`** file contains the complete project workflow including:

- Data exploration and visualization
- Exploratory Data Analysis (EDA)
- Feature scaling and preprocessing
- Model training and hyperparameter tuning
- Cross-validation results
- Performance evaluation
- Model serialization

This notebook is useful for understanding the full development process and can be run in Google Colab.

---

## 👨‍💻 Author

**Emmanuel Ejima**

Chemical Engineer | Data Science & Machine Learning Enthusiast | Renewable Energy Engineer

- **GitHub:** https://github.com/EmmanuelEjima
- **LinkedIn:** https://linkedin.com/in/emmanuel-ejima
- **Portfolio:** https://github.com/EmmanuelEjima/Data-Science-Machine-Learning-Portfolio

---

⭐ **If you found this project useful, consider giving it a Star on GitHub!**
