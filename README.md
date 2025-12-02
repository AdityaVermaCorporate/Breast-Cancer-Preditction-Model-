🔬 Breast Cancer Classification Model — Project Description
This project focuses on building a high-performance Breast Cancer Classification model using XGBoost, with an emphasis on real-world deployment, feature interpretability, and rigorous evaluation.
During the development, I explored two alternative modeling strategies:
Real-world deployment approach:
Using SHAP to identify the most influential features and training a lightweight model optimized for practical use.
This reduced model complexity and improved interpretability, though with a slight trade-off in accuracy.
High-accuracy approach:
Training an XGBoost classifier using all available features to maximize predictive power.
This version prioritizes pure performance and was extensively tuned.
⚙️ Process & Methodology
Data Exploration:
Visualized thousands of rows using box plots for each parameter and interactive pair plots with plotly.express to understand feature relationships and detect skew/outliers.
Feature Engineering:
Created and transformed multiple columns to enhance feature integration and strengthen the model’s learning ability.
Model Training:
Implemented XGBoost Classifier, optimizing performance through hyperparameter tuning across various parameters (learning rate, max depth, estimators, subsample, etc.).
Evaluation:
Assessed models using:
ROC-AUC Curve (aimed for near-perfect separation)
Precision-Recall Curve
Accuracy, Precision, Recall, and F1-Score
These metrics helped compare the minimal-feature model vs full-feature model.
Interpretability:
Used SHAP values to understand how individual features contribute to predictions and support decision-making transparency.
