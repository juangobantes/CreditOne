[README_CreditOne.md](https://github.com/user-attachments/files/21622946/README_CreditOne.md)

# 💳 CreditOne: Loan Default Risk Modeling

This project aims to develop a predictive model that helps **CreditOne**, a financial service provider, assess customer creditworthiness and reduce loan default risk. It follows a full data science workflow, from data exploration to model evaluation.

## 🎯 Objective

Design a machine learning model that accurately predicts whether a customer will default on a loan, enabling more informed and profitable lending decisions.

## 📁 Dataset

- **Source**: Provided by CreditOne (based on the Taiwan credit default dataset)
- **Rows**: 3,670
- **Target Variable**: `Y` – binary classification (`default`, `not default`)
- **Features**:
  - `LIMIT_BAL`: Credit limit
  - `SEX`, `EDUCATION`, `MARRIAGE`, `AGE`: Customer demographics
  - `PAY_0` to `PAY_6`: Payment status (past 6 months)
  - `BILL_AMT1` to `BILL_AMT6`: Monthly bill amounts
  - `PAY_AMT1` to `PAY_AMT6`: Monthly payment amounts

## 🧪 Project Workflow

### 1. Problem Framing
- Business risk identified: rise in loan defaults
- Goal: classify credit applicants into `default` or `not default` categories

### 2. Data Preparation
- Renamed columns using first row headers
- Cleaned `Unnamed: 0` and reset index
- Checked for missing values and data types

### 3. Exploratory Data Analysis (EDA)
- Distribution of demographic and financial variables
- Correlation heatmaps to detect influential features
- Balance of target classes

### 4. Modeling
- Applied supervised machine learning techniques:
  - Logistic Regression
  - Random Forest
  - [Include others if used: e.g., XGBoost, SVM]
- Train-test split and cross-validation used for evaluation

### 5. Model Evaluation
- Metrics: Accuracy, Precision, Recall, F1-score
- Confusion Matrix and ROC-AUC to assess performance
- Feature importance plots to identify key drivers

## 🔍 Key Insights

- Key predictors of default include recent payment history (`PAY_0`–`PAY_6`) and current balance (`BILL_AMTx`)
- Logistic Regression provided explainability, while Random Forest improved accuracy

## 🛠️ Tools & Libraries

- Python (Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn)
- Jupyter Notebook

## 📂 Files in this Repository

- `Entregable-Copy1.ipynb` – Main analysis notebook
- `Credit_one_df.csv` – Cleaned dataset

## 🚀 Future Enhancements

- Hyperparameter tuning using GridSearchCV
- Deployment as a web app using Streamlit or Flask
- Add SHAP/LIME for model interpretability
- Extend dataset to include more behavioral attributes

## 📬 Contact

**Juan María Gobantes Gómez**  
🔗 [LinkedIn](https://www.linkedin.com/in/juanmariagobantesgomez/) | 💻 [GitHub](https://github.com/juangobantes)
