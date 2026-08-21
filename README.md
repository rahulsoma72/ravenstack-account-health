# RavenStack PM Account Health Tool

This Streamlit application is the PM-facing implementation of the
frozen Random Forest model from the RavenStack dissertation.

Final features:
- account_age_days
- subscription_tenure_days
- days_since_latest_subscription_start

Training CV ROC-AUC: 0.6654 ± 0.0613
Final test ROC-AUC: 0.6148
Final test PR-AUC: 0.5085

The application does not retrain the model, use XGBoost, use SMOTE,
or tune against the test set.

## Files

- app.py
- requirements.txt
- ravenstack_final_random_forest_model.joblib
- ravenstack_pm_accounts.csv
- ravenstack_pm_features.csv

## Run locally

pip install -r requirements.txt
streamlit run app.py

## Deploy

Push the files to GitHub and deploy app.py using Streamlit Community Cloud.
