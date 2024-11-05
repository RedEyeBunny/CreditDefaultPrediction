# Problem Definition

Financial institutions face significant challenges when assessing the creditworthiness of loan applicants. Approving loans for high-risk applicants can lead to losses due to defaults, while rejecting low-risk applicants can result in missed revenue opportunities. The goal of this project is to address this issue by building a predictive model that can:

1. Classify loan applicants into "default" and "non-default" categories based on historical data.
2. Help financial institutions reduce financial losses by identifying high-risk applicants
3. Enhance the loan approval process by incorporating data-driven risk assessment into decision-making.

# Results

1. Accuracy: The model achieved an accuracy score of around 0.83.
2. AUC-ROC Score: After tuning, the AUC-ROC score reached 0.9022, indicating strong discriminatory power between default and non-default borrowers.
3. Cross-Validation Results: With cross-validation, the mean AUC-ROC score was approximately 0.897, with a standard deviation of 0.006, indicating consistent performance across folds.

These results demonstrate that the model can effectively predict credit risk, with high reliability and accuracy.

# Key Insights

1. loan_grade and monthly_payment_36Months are the most significant predictors of loan default.
2. Higher loan grades and monthly payments correlate positively with the likelihood of default, while higher income generally reduces default risk.
3. Feature importance analysis using SHAP values helps explain the model's predictions, making the model more interpretable and valuable for decision-makers.

# Future Work

To further improve the model, we can:

1. Experiment with additional models, like Random Forest and LightGBM, for comparison.
2. Collect and integrate more features, such as credit score, debt-to-income ratio, and loan term.
3. Use more advanced hyperparameter tuning techniques, like Bayesian Optimization, for potentially better results.
