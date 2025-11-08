# Logistic-Regression
After completing this lab you will be able to:  * Use Logistic Regression for classification * Preprocess data for modeling * Implement Logistic regression on real world data


## Logistic Regression for Telco Customer Churn Prediction

This Jupyter notebook implements a complete **Logistic Regression classification model** to predict customer churn in the telecommunications industry using Python and scikit-learn. The project demonstrates end-to-end machine learning workflow including data preprocessing, model training, evaluation, and feature importance analysis.[1]

### Project Overview

This implementation focuses on predicting which customers are likely to leave a telecommunications company's land-line business for cable competitors. The model achieves approximately **66% accuracy** through logistic regression classification and provides insights into the key factors influencing customer churn.[1]

### Dataset

The project uses the **Telco Customer Churn dataset**, a hypothetical dataset representing telecommunications customer data. The dataset contains 200 customer records with 28 features including:[1]

**Demographic Features:**
- tenure: Length of customer relationship
- age: Customer age
- address: Years at current address
- income: Annual income
- ed: Education level (1-5 scale)
- employ: Years with current employer

**Service Features:**
- equip: Equipment rental (binary)
- callcard: Calling card service (binary)
- wireless: Wireless service (binary)

**Target Variable:**
- churn: Customer churn indicator (0=retained, 1=churned)[1]

The dataset exhibits a **29% churn rate** (58 out of 200 customers), providing a realistic business scenario for classification modeling.[1]

### Key Features

**Data Preprocessing:**
- Feature selection and subset extraction
- Data type conversion for target variable
- **StandardScaler normalization** for feature scaling
- Train-test split (80-20 ratio) with random state for reproducibility[1]

**Model Implementation:**
- Logistic Regression classifier from scikit-learn
- Model training on standardized features
- Prediction and probability estimation
- **Log-loss evaluation metric** for model performance assessment[1]

**Analysis & Visualization:**
- Feature coefficient visualization using horizontal bar plots
- Interpretation of coefficient magnitudes and directions
- Probability-based prediction analysis
- Feature importance ranking for business insights[1]

### Technical Stack

- **Python 3.12.4**
- **pandas 2.2.3**: Data manipulation and analysis
- **numpy 2.2.0**: Numerical computing
- **scikit-learn 1.6.0**: Machine learning algorithms and preprocessing
- **matplotlib 3.9.3**: Data visualization[1]

### Model Performance

The trained model achieves a **log-loss of approximately 0.626** on the test set, indicating reasonable predictive performance. Log-loss (logarithmic loss or binary cross-entropy) measures the performance of a classification model where predictions are probability values between 0 and 1 - lower values indicate better model performance.[1]

### Feature Importance Insights

The model provides interpretable coefficients for each feature, where:
- **Large positive coefficients** indicate that increases in the feature value lead to higher churn probability
- **Large negative coefficients** indicate that increases in the feature value lead to lower churn probability
- **Small absolute values** suggest weaker influence on churn prediction[1]

The visualization clearly shows which customer attributes have the strongest impact on churn decisions, enabling data-driven retention strategies.[1]

### Usage

The notebook provides a complete, executable workflow that can be run sequentially from top to bottom. Key sections include:[1]

1. Library installation and imports
2. Data loading and exploration
3. Feature engineering and preprocessing
4. Data standardization
5. Train-test splitting
6. Model training
7. Prediction generation
8. Performance evaluation
9. Feature coefficient analysis and visualization

### Practice Exercises

The notebook includes hands-on exercises to explore model behavior with different feature combinations:
- Adding individual features (callcard, wireless)
- Removing features (equip, income, employ)
- Analyzing the impact on log-loss performance[1]

### Learning Objectives

After completing this implementation, users will be able to:
- Use Logistic Regression for binary classification tasks
- Preprocess data for machine learning modeling
- Implement end-to-end ML pipelines
- Evaluate model performance using appropriate metrics
- Interpret model coefficients for business insights[1]

### Estimated Completion Time

**60 minutes**[1]

### Applications

This implementation is ideal for:
- Customer churn prediction in telecommunications and subscription-based businesses
- Educational purposes for learning classification techniques
- Foundation for more advanced customer retention models
- Business intelligence and customer analytics projects[1]

## Dataset link: https://www.kaggle.com/datasets/ezzaldeenesmail/telco-churn-dataset/data
