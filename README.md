Predicting User Ad Clicks Using Machine Learning 📊🧠

Author: Swapnil Herwadkar

Tech Stack: Python, Scikit-Learn, XGBoost, SMOTE, Pandas, Matplotlib

🔍 Overview
This project presents a machine learning pipeline for predicting whether a user will click on an online ad, based on behavioral and demographic data. By applying robust preprocessing, handling class imbalance with SMOTE, and optimizing models like XGBoost, this project aims to improve digital ad targeting and maximize click-through rates.

🎯 Objectives
Predict ad click-through behavior using user features and ad context.

Handle severe class imbalance to better identify the minority (clicked) class.

Engineer interaction features to enhance model performance.

Evaluate and compare model performance using classification metrics.

🛠️ Methods & Techniques
1. 🧹 Data Preprocessing
Dropped irrelevant features (e.g., ID, full name).

One-hot encoding for categorical variables (e.g., device type, ad position).

Created interaction terms to capture contextual behavior (e.g., device_type × time_of_day).

2. ⚖️ Class Imbalance Handling
Applied SMOTE (Synthetic Minority Over-sampling Technique) to balance the dataset and improve recall for rare events (ad clicks).

3. 🤖 Models Used
Logistic Regression (baseline)

Random Forest (ensemble model)

XGBoost (best performer after hyperparameter tuning)

4. 🎯 Evaluation Metrics
Accuracy, Precision, Recall

Confusion Matrix

ROC-AUC Curve

📈 Key Results
XGBoost achieved the highest performance post-SMOTE and hyperparameter tuning.

Visualization of class balance before/after SMOTE showed significant improvements in model learning.

Feature interactions (e.g., ad_position × browsing_history) played a key role in performance gains.

📌 Visualizations
Bar plots for performance metrics

Confusion matrices per model

ROC curves comparing classifiers

Class distribution before and after SMOTE

💡 Insights & Recommendations
Time of Day, Device Type, and Ad Position are highly predictive features.

SMOTE was critical in overcoming class imbalance and improving minority class recall.

This framework can be deployed in real-time ad platforms to dynamically adjust ad placement and content.

🚀 Future Improvements
Incorporate time zone and session-based behavior.

Deploy as a REST API for real-time predictions.

Experiment with deep learning models for higher granularity.
