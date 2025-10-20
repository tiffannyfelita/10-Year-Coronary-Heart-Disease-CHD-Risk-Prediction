# 10-Year-Coronary-Heart-Disease-CHD-Risk-Prediction
##  Project Overview
This **group project** aims to **predict the 10-year risk of coronary heart disease (CHD)** using patient demographic, behavioral, and medical data.  
The dataset includes features such as age, sex, smoking habits, blood pressure, cholesterol, BMI, glucose, and medical history.  
Machine learning models are applied to classify whether a patient is at high risk (`1`) or low risk (`0`) of developing CHD within ten years, supporting early detection and preventive healthcare interventions.

## Model: Stacking Classifier
A **Stacking Classifier** is used to improve predictive performance by combining multiple base models.

### Base Estimators
- **Logistic Regression:** A linear model used for binary classification, serving as a simple baseline learner.  
- **Random Forest:** An ensemble of decision trees (`max_depth=10`, `n_estimators=300`) that captures non-linear relationships in the data.  
- **SVC (Support Vector Classifier):** A linear kernel SVM (`C=0.1`) that separates classes using a hyperplane.

### Final Estimator
- **Logistic Regression:** Combines the predictions of the base estimators to produce the final output, learning the optimal weights for each base model.

> This stacking approach leverages the strengths of different models, improving overall accuracy and robustness compared to individual classifiers.

## Tech Stack
- **Languages & Frameworks:** Python, scikit-learn  
- **Libraries:** NumPy, Pandas, Matplotlib, Seaborn  
