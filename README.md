# Easy Visa – Visa Case Prediction using Ensemble Learning

**Project Overview**

The Easy Visa project is a machine learning-based classification system designed to predict the outcome of visa applications (Certified or Denied). Leveraging ensemble learning techniques such as Bagging, Boosting, Random Forest, XGBoost, and Stacking, the model aims to identify patterns that influence visa approvals, assisting legal professionals and applicants alike.

**Problem Statement**
Visa approval processes can be unpredictable and time-consuming. Automating the classification of visa applications can provide early insights, reduce manual effort, and enhance transparency. This project classifies visa cases based on application features using multiple ensemble-based machine learning models.

**Dataset**

- Total Records: 25,480
- Features: 10 initial columns (including employer, job title, wages, etc.)
- Target Variable: case_status (Mapped to 0 = Denied, 1 = Certified)
- Class Distribution:
    - Training Set (70%): 66.7% Certified, 33.3% Denied
    - Test Set (30%): 66.9% Certified, 33.1% Denied

**Workflow**

**1. Exploratory Data Analysis (EDA)**

- Visualized target distribution
- Analyzed missing values and feature correlations
- Identified categorical and numerical columns

**2. Feature Engineering**

- Mapped target variable (Certified → 1, Denied → 0)
- One-hot encoded categorical variables
- Converted Boolean features to 0 and 1
- Split dataset into training and testing sets

**3. Model Evaluation Metrics**

Used the following metrics for evaluation:
- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix (Visualized with heatmaps)

**4. Ensemble Models Built**

- Decision Tree
- Bagging Classifier
- Random Forest
- AdaBoost
- Gradient Boosting
- XGBoost
- Stacking Classifier

**Results:**
 XGBoost (Tuned) is the Best: Highest F1 Score: At 0.8256, it outperforms all other models on the test set, balancing both precision and recall effectively.

**Feature Importance (from XGBoost)**
The most influential features were visualized using XGBoost’s feature_importances_. This helped identify key factors influencing visa approval outcomes
