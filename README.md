# Waze User Churn Prediction Project

## Project Overview
This project aims to predict user churn for Waze using machine learning models. The primary goal is to identify the factors driving user churn and to build predictive models that can help Waze improve user retention. Two tree-based models, Random Forest and XGBoost, are built and tested to achieve the best results.

## Project Structure
The project is divided into several key parts:

1. **Ethical Considerations**
   - Assessment of ethical implications and consequences of model errors.

2. **Feature Engineering**
   - Selection, extraction, and transformation of features for modeling.

3. **Modeling**
   - Building and evaluating Random Forest and XGBoost models.

## Data
The dataset used in this project consists of various user interaction metrics with Waze. Key features include:
- Sessions
- Drives
- Total Sessions
- Days after Onboarding
- Total Navigations to Favorite Places
- Driven Kilometers
- Duration in Minutes
- Activity Days
- Driving Days
- Device Type

## Steps and Instructions

### 1. Ethical Considerations
Reflect on the potential ethical implications of predicting user churn and the impact of false positives and false negatives on users.

### 2. Feature Engineering
Create new features to enhance model performance, such as:
- Kilometers per Driving Day
- Percent of Sessions in Last Month
- Professional Driver Indicator
- Total Sessions per Day
- Kilometers per Hour
- Kilometers per Drive
- Percent of Drives to Favorite Places

### 3. Data Preparation
- Load and inspect the dataset.
- Handle missing values and outliers.
- Encode categorical variables.

### 4. Modeling
- Split data into training, validation, and test sets.
- Train and tune Random Forest and XGBoost models using GridSearchCV.
- Evaluate model performance based on recall, precision, F1 score, and accuracy.

### 5. Model Evaluation
- Compare models using validation data.
- Select the champion model (XGBoost) based on performance metrics.
- Test the champion model on the test data.

### 6. Feature Importance
- Plot feature importance for the XGBoost model to understand which features contribute most to the predictions.

### 7. Decision Threshold Optimization
- Explore different decision thresholds to optimize recall and precision based on business needs.

## Results
- The XGBoost model outperformed the Random Forest model, achieving better recall and F1 scores.
- Feature engineering significantly improved model performance, with engineered features accounting for many of the top predictive features.

## Conclusion
- The model can help guide further exploratory efforts to improve user retention strategies.
- Ethical considerations should be addressed to mitigate any negative impact on users due to model predictions.

## Future Work
- Further feature engineering and data collection can improve model accuracy.
- Explore additional modeling techniques and ensemble methods.
- Conduct follow-up analyses on the effectiveness of proactive retention measures.

## Dependencies
- Python 3.x
- pandas
- numpy
- matplotlib
- scikit-learn
- xgboost


