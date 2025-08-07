# Credit-default-prediction-taiwan
Predicting credit card payment defaults in Taiwan using EDA, data preprocessing, and classification models including logistic regression and decision trees. Insights were drawn from demographic and financial patterns to help improve credit risk analysis.
# Credit Card Default Prediction in Taiwan

This project analyzes and predicts default behavior of credit card clients in Taiwan using statistical techniques, Exploratory Data Analysis (EDA), and machine learning algorithms. The dataset, obtained from a research study, is rich with financial and demographic details of 30,000 clients, allowing a deep dive into credit risk factors.

---

## 📊 Project Overview

**Course**: ALY6140 – Python and Analytics Systems Technology  
**Professor**: Wada Roy  
**Submission Date**: December 17, 2023

The main goal is to explore the factors that contribute to a customer defaulting on their credit card payment the next month. Using classification models and visual analysis, we examine relationships between variables like age, sex, education, payment history, bill amounts, and more.

---

## 📁 Dataset Summary

- **Source**: UCI Machine Learning Repository
- **Total Records**: 30,000
- **Features**: 24 independent variables + 1 target variable (`default payment next month`)
- **Key Variables**:
  - `LIMIT_BAL`: Credit limit
  - `SEX`, `EDUCATION`, `MARRIAGE`: Demographic information
  - `PAY_0` to `PAY_6`: Repayment status for last 6 months
  - `BILL_AMT1` to `BILL_AMT6`: Historical bill amounts
  - `PAY_AMT1` to `PAY_AMT6`: Historical payment amounts
  - `default payment next month`: Target variable (0 = No, 1 = Yes)

---

## 🔍 Business Questions

1. **Credit Risk Assessment**
   - What factors most strongly associate with default?
   - Can patterns be detected for early identification?

2. **Customer Segmentation**
   - How does spending vary by gender, age, or marital status?
   - Are some demographic segments more likely to default?

---

## 🧹 Data Cleaning

- Checked for null values and duplicates.
- Handled approximately 10% inconsistencies.
- Encoded categorical variables for modeling.
- Verified unique entries using the `ID` column.

---

## 📈 Exploratory Data Analysis (EDA)

- **Univariate Analysis**: 
  - Histograms and bar plots for education, age, and gender.
- **Bivariate Analysis**: 
  - Count plots comparing demographic features to default behavior.
  - Histograms showing distribution of age and credit limit by default status.
- **Heatmap**: 
  - Showed strong correlation among repayment and bill amount features.

---

## 🧠 Modeling Approach

### 1. **Logistic Regression**
- Used to interpret feature importance in predicting default.
- Evaluated with classification report and accuracy score.

### 2. **Decision Tree Classifier**
- Provided easy-to-understand visual interpretation.
- Compared performance with logistic regression.

---

## 📊 Key Insights

- Male clients dominate the “Married + University” segment with higher default rates.
- Single females in university tend to have a lower risk profile.
- Default probability correlates with repayment delays (`PAY_0` to `PAY_6`).
- Larger bill amounts are not always predictive unless combined with poor payment history.

---

## 🧰 Tools Used

- Python
- pandas, numpy
- matplotlib, seaborn
- scikit-learn

---

## 📌 Future Work

- Apply more advanced models (e.g., Random Forest, XGBoost).
- Use cross-validation for robust model evaluation.
- Add SHAP/feature importance plots to interpret model predictions.

---

## 📎 References

- [UCI Machine Learning Repository: Default of Credit Card Clients Dataset](https://archive.ics.uci.edu/ml/datasets/default+of+credit+card+clients)
- Internal course material and lectures (Northeastern University)

---

## 👩‍💻 Author

**Anoushka Hazari**  
