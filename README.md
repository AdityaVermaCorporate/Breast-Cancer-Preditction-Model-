🩺 Breast Cancer Classification Using XGBoost & SHAP
A machine learning project focused on accurately predicting breast cancer diagnoses using XGBoost, SHAP-based interpretability, extensive visualization, and advanced model tuning.
This repository includes both a real-world deployable model (reduced features, interpretable) and a high-accuracy full-feature model.
📌 Project Overview:

The primary goal of this project is to build and evaluate breast cancer classification models while balancing accuracy, interpretability, and real-world usability.
During development, two modeling strategies were explored:

1️⃣ Deployable, interpretable model: 

Selected top features using SHAP value analysis
Trained a lightweight model with fewer features
Improved interpretability and practicality
Slight reduction in accuracy (intentional trade-off)

2️⃣ High-accuracy model:

Used all available features
Trained an XGBoost Classifier
Performed extensive hyperparameter tuning
Achieved excellent performance on ROC-AUC and Precision-Recall metrics

🔍 Data Exploration & Visualization:

Before modeling, the dataset was analyzed deeply through:
Box plots for detecting outliers, distribution spread, and skew
Interactive pair plots built with plotly.express to understand relationships between features
Correlation analysis to detect multicollinearity
Feature engineering to enhance pattern extraction and model learning

⚙️ Modelling Process:

Feature Engineering
Created additional columns and transformations
Improved feature integration and model expressiveness
Model Training
Implemented XGBoost Classifier
Tuned parameters including:
learning rate
max_depth
n_estimators
subsample
colsample_bytree
gamma
Used a train–test split to ensure fair evaluation

📈 Evaluation Metrics:

Both models were assessed using:
ROC-AUC Curve (primary metric for separation quality)
Precision-Recall Curve
Accuracy, Precision, Recall, and F1-Score
Confusion Matrix for understanding real-world misclassifications
The full-feature model achieved exceptional ROC-AUC and precision scores, while the reduced-feature model remained effective and deployment-friendly.

🧠 Model Interpretability:

SHAP (SHapley Additive exPlanations) was used to:
Understand how each feature impacts predictions
Rank features by importance
Validate whether reduced-feature models still contain the strongest predictors
Support real-world decision transparency
✅ Project Outcomes
High-performance model optimized through hyperparameter tuning
Simplified, interpretable model built specifically for practical deployment
Extensive visual insights into data patterns and feature relationships
Clean end-to-end ML workflow from EDA → Feature Engineering → Tuning → Evaluation

📂 Technologies Used:

Python
XGBoost
SHAP
Plotly Express
NumPy & Pandas
Matplotlib / Seaborn
🚀 Future Improvements
Deployment through FastAPI or Flask
Real-time prediction interface
Model comparison dashboard
SHAP visual reports for clinicians
