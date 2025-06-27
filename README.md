Give Me Some Credit: Nutritional Labels for Automated Decision Systems
This project focuses on building and evaluating a machine learning system for predicting the probability that a borrower will experience financial distress within two years. Using the "Give Me Some Credit" dataset of 250,000 borrower records, we developed multiple models and analyzed their fairness to produce an interpretable and responsible credit scoring system.

 Project Goals
Predict financial distress using historical borrower data.

Improve data quality through preprocessing and imputation.

Evaluate model performance and fairness across income groups.

Mitigate algorithmic bias using fairness-aware techniques.

 Implementation Highlights
Data Cleaning & Imputation: Handled missing values using iterative imputation and optimized memory usage.

Feature Engineering: Applied binning, discretization, and Weight of Evidence (WOE) encoding.

Modeling: Trained models using Logistic Regression, XGBoost, LightGBM, CatBoost, and Gaussian Naive Bayes.

Bias Mitigation: Used AIF360’s DisparateImpactRemover and fairness metrics (e.g., disparate impact, mean difference).

Evaluation: ROC AUC, accuracy, and fairness metrics guided model selection and ensemble stacking.

 Fairness & Ethical Considerations
A core goal was to balance accuracy with fairness. We created a binary_income attribute to analyze disparate impact across privileged (high income) and unprivileged (low income) groups, experimenting with mitigation strategies to reduce bias.

 Tech Stack
Python, Pandas, NumPy, Scikit-learn

XGBoost, LightGBM, CatBoost

AIF360 (IBM AI Fairness 360 Toolkit)

Matplotlib, Seaborn (for visualization)

 Files
Project_Implementation.ipynb: Main modeling and pipeline development notebook

Outcomes*.ipynb: Fairness analysis and ROC curve visualization

ADS Report.pdf: Full project write-up and methodology documentation

 Dataset
Dataset used: Give Me Some Credit – Kaggle
https://www.kaggle.com/c/GiveMeSomeCredit/overview
