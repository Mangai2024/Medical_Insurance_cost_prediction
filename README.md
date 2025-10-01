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
With Feature Engineering (Random Forest)

Random Forest (with FE)

MAE: 2835.53

RMSE: 4494.85

R²: 0.8139

🔍 Insights

Smoking has the highest impact on insurance charges.

BMI and Age interact strongly with smoking habits.

Random Forest (tuned) gave the best performance with R² = 0.83.

Feature Engineering improved interpretability but did not outperform tuned Random Forest in score (still useful for interview explanation).

🚀 Future Improvements

Apply hyperparameter tuning with RandomizedSearchCV / GridSearchCV

Perform cross-validation for robust estimates

Try log-transform of target (charges) to reduce skewness

Deploy as a simple web app (Streamlit / FastAPI) for real-world usage

📝 Conclusion

This project demonstrates how machine learning can predict medical insurance costs effectively. Among all models tested, Random Forest Regressor with hyperparameter tuning achieved the best performance (R² ≈ 0.83). Feature engineering provided interpretability and domain insights, which are crucial in practical applications even if the score didn’t improve further.
