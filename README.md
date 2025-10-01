🏥 **Medical Insurance Cost Prediction**

This project predicts medical insurance charges using demographic and lifestyle factors such as age, BMI, children, smoking status, and region.

📌 **Problem Statement**

Health insurance companies need accurate models to estimate individual medical costs. The objective of this project is to build and compare machine learning models that can predict these charges reliably.

📂 **Dataset**

Source: Medical Cost Personal Dataset (commonly on Kaggle)

**Features:**

age → Age of the individual

sex → Gender

bmi → Body Mass Index

children → Number of dependents

smoker → Smoking habit

region → Residential area

Target:

charges → Insurance cost (USD)

🧾 Workflow

**Data Preprocessing 🧹
**
Handled missing values

Encoded categorical variables

Train-test split

Exploratory Data Analysis (EDA) 📊

Studied distributions of age, BMI, charges

Compared smoker vs non-smoker charges

Observed correlations

Feature Engineering (FE) ⚙️

Added interaction features: bmi × smoker, age × smoker

Added non-linear features: bmi², age²

Created bins: age_bin, bmi_cat

One-hot encoded categorical variables

**Modeling 🤖
**
Linear Regression (baseline)

Random Forest Regressor

**XGBoost Regressor**

Model Evaluation 📏

Metrics: MAE, RMSE, R²

📊 Results
🔹 Without Feature Engineering

**Linear Regression**

MAE: 3733.41

RMSE: 5514.35

R²: 0.7199

Random Forest (Tuned)

MAE: 2349.20

RMSE: 4298.44

R²: 0.8298

XGBoost

MAE: 2373.77

RMSE: 4924.08

R²: 0.7766

🔹 With Feature Engineering (Random Forest)

**Random Forest (with FE)**

MAE: 2835.53

RMSE: 4494.85

R²: 0.8139

🔍 Insights

🚬 Smoking has the highest impact on insurance charges

📈 BMI and Age interact strongly with smoking habits

🌲 Random Forest tuned gave the best performance with R² ≈ 0.83

🧠 Feature Engineering improved interpretability but did not outperform tuned Random Forest in score

🚀 ****Future Improvements**
**
🔧 Apply hyperparameter tuning with RandomizedSearchCV or GridSearchCV

🔄 Perform cross-validation for robust estimates

📉 Try log-transform of target (charges) to reduce skewness

🌐 Deploy as a simple web app (Streamlit or FastAPI)

📝**** **Conclusion********
**
This project demonstrates how machine learning can predict medical insurance costs effectively.
Among all models tested, Random Forest Regressor with hyperparameter tuning achieved the best performance (R² ≈ 0.83).
Feature engineering provided interpretability and domain insights, which are important in practical applications even if the score did not improve further.
