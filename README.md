# 🇮🇳 Indian Election 2019 Candidates Data Analysis

This project explores and analyzes the open-source dataset of candidates who contested the **Indian General Election 2019**, containing 2,263 records across various states, constituencies, and political parties.

📊 The goal was to perform **end-to-end data preprocessing, encoding, imputation, discretization, outlier handling, and feature selection** to extract meaningful insights and enable downstream modeling and analytics.

---

## 🔗 Dataset

[Kaggle Dataset – Indian Candidates for General Election 2019](https://www.kaggle.com/datasets/prakrutchauhan/indian-candidates-for-general-election-2019)

---

## 🛠️ Techniques Used

- **Missing Value Analysis & Cleaning**: Handled nulls using complete case analysis (CCA) and imputation (mean, median, mode).
- **Feature Engineering**:
  - Converted string-encoded monetary fields like `ASSETS`, `LIABILITIES` to numeric.
  - Encoded categorical variables using:
    - Label Encoding (`STATE`, `CONSTITUENCY`)
    - Frequency Encoding (`PARTY`)
    - One-Hot Encoding (`CATEGORY`)
    - Ordinal Encoding (`EDUCATION`, `GENDER`)
- **Discretization**:
  - KMeans clustering on `TOTAL ELECTORS`
  - Decision Tree Binning on `AGE`
- **Outlier Handling**:
  - Identified extreme values via boxplots
  - Applied capping using IQR-based thresholds
- **Feature Scaling**:
  - Z-score standardization and Min-Max normalization on skewed variables
- **Feature Selection**:
  - Chi-Squared Test to identify top predictors of winning (`WINNER`)
  - Correlation Heatmap for multivariate analysis
- **Data Visualization**:
  - Histograms, bar plots, and heatmaps for pattern recognition and feature distribution

---

## 🔍 Key Insights

- Assets and education level of candidates show significant variation and potential impact on election outcomes.
- Some constituencies like Malkajgiri have outlier-level electorate sizes, affecting representativeness.
- Party affiliations exhibit high imbalance, making frequency encoding more effective.
- Preprocessing and feature selection improved interpretability and prepared the dataset for predictive modeling.

---

## ✅ Skills Demonstrated

- **Technical**: Python, Pandas, Scikit-learn, Matplotlib, Seaborn, Feature Engineering, EDA, Encoding, Imputation
- **Analytical**: Critical thinking, data cleaning, insight extraction, correlation analysis
- **Soft Skills**: Problem solving, reproducibility, documentation

---

> 📌 This project is part of my portfolio demonstrating practical data preprocessing, analytics, and feature engineering on real-world datasets.

