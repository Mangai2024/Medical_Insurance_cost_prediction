Medical Insurance Cost Prediction

This project predicts medical insurance charges based on demographic and lifestyle factors such as age, sex, BMI, number of children, smoking status, and region.

📌 Problem Statement

Insurance companies need accurate methods to estimate the medical costs of individuals. This project uses machine learning models to build predictive systems that provide reliable estimates of insurance charges.

📂 Dataset

Source: Medical Cost Personal Dataset (commonly available on Kaggle)

Features: age, sex, bmi, children, smoker, region

Target: charges (medical insurance cost)

🧾 Workflow

Data Preprocessing – encoded categorical features, scaled numerical values, and split data into train/test.

Exploratory Data Analysis (EDA) – studied how smoking, BMI, and age influence insurance charges.

Model Building – trained and compared Linear Regression, Random Forest, and XGBoost.

Model Evaluation – measured performance using MAE, RMSE, and R².

📊 Model Results

Linear Regression

MAE: 3733.41

RMSE: 5514.35

R²: 0.7199

Random Forest Regressor

MAE: 2504.47

RMSE: 4727.66

R²: 0.7941

XGBoost Regressor

MAE: 2373.77

RMSE: 4924.08

R²: 0.7766

🔍 Insights

Smoking is the strongest driver of higher insurance costs.

BMI and age also significantly influence charges.

Random Forest performed the best overall with the highest R² (0.7941).

XGBoost was slightly behind Random Forest but still performed better than Linear Regression.

Linear Regression served as a good baseline but struggled with non-linear relationships in the data.
