# Explainable AI Study on Identifying Factors Affecting Customer Churn

This project presents a comprehensive, explainable AI (XAI) approach to understanding and predicting customer churn. As a data scientist, the goal was to identify key factors contributing to churn through a rigorous end-to-end pipeline involving data preprocessing, feature engineering, model selection, and interpretability.

## 📊 Project Overview

Customer churn is a critical metric in subscription-based industries. Using a real-world dataset, this project explores various preprocessing techniques, feature selection methods, and machine learning models to predict churn with a focus on interpretability.

Key objectives:
- Identify and rank key features contributing to churn.
- Evaluate and compare different model performances.
- Apply explainable AI techniques for model transparency.

---

## 🧰 Tools & Technologies

- **Python**
- **Pandas, NumPy, Scikit-learn**
- **XGBoost, Random Forest, SVM, Logistic Regression**
- **SMOTE** for imbalanced data handling
- **PCA, Chi-Square, Mutual Information, RFE, LASSO** for feature selection
- **SHAP** (if included in the notebook) for interpretability

---

## 🧪 Methodology

### 1. Data Preprocessing
- Handling missing values
- Encoding categorical variables (Frequency, One-Hot)
- Scaling and imputing numerical features
- SMOTE for balancing classes

### 2. Feature Engineering
- Equal binning of numerical features
- Binary conversion for categorical columns

### 3. Feature Selection Techniques
- **PCA** (Dimensionality Reduction)
- **Filter Methods**: Correlation, Chi-square, Mutual Information
- **Wrapper Method**: Recursive Feature Elimination (RFE)
- **Embedded Method**: LASSO Regression

### 4. Model Training & Evaluation
- Trained models on different feature sets
- Compared performance on:
  - PCA-transformed data
  - Filtered feature set
  - Wrapped feature set
  - Embedded feature set
- Best performing models: **Random Forest** and **XGBoost** (Filtered features)
- Overfitting identified with some models using Wrapper and Embedded methods

---

## 🧠 Explainability

Explainable AI methods are used to:
- Understand model decision logic
- Provide feature importance
- Improve trust and transparency in predictive results

---

## 📈 Results

- **Best Accuracy**: ~91% with Random Forest and XGBoost
- **Key Insight**: Filter-based feature selection provided the most balanced model performance
- Models using PCA or overfitted Wrapper/Embedded features lacked generalization

---

## 🚀 Getting Started

1. Clone the repo:
   ```bash
   git clone https://github.com/pd-bds/Explainable-AI-Study-on-Identifying-Factors-Affecting-Customer-Churn.git
   cd Explainable-AI-Study-on-Identifying-Factors-Affecting-Customer-Churn
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the notebook or script to reproduce results.

---

## 📚 References

- Scikit-learn documentation
- XGBoost user guide
- Research papers on customer churn prediction and XAI

---

## 🙌 Acknowledgments

Thanks to the open-source community for the tools and libraries used in this project.
