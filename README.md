# Credit Risk Analysis and Default Prediction
## Goal
The goal of this project is to analyze and predict loan defaults using a credit risk dataset. By identifying key risk factors and building predictive models, we aim to provide insights into customer behavior and assess the likelihood of default. This analysis can assist financial institutions in decision-making processes, risk mitigation, and improving lending strategies.

## Project Overview
This project is divided into several stages:

## 1. Exploratory Data Analysis (EDA)
Data Cleaning:
- Handled missing data in the Emp_length and Rate columns using median imputation to avoid biases caused by outliers.
- Removed duplicate rows and handled invalid or extreme outlier values in Age and Emp_length.
  
Visualization:
- Created box plots and count plots to identify outliers and understand distributions.
- Categorized customers into Age_Group bins to facilitate group-based analysis.
- Analyzed the count and distribution of loan defaults by various attributes.

## 2. Feature Engineering
Derived new features, such as Age_Group and Risk_Level, to enhance predictive capabilities:
- Risk_Level: Categorized loans into "Low", "Medium", and "High" risk based on interest rates.
  
One-hot encoded categorical variables for modeling compatibility.

## 3. Data Analysis
Default Rate Analysis:
- Examined default rates across key dimensions such as Age_Group, Home Ownership, and Risk_Level.
- Visualized these relationships using bar plots to provide actionable insights.
Correlation Analysis:
- Used a heatmap to evaluate relationships between numerical features.
  
## 4. Predictive Modeling
Implemented three machine learning models for predicting loan default:
- Logistic Regression
- Random Forest Classifier
- Gradient Boosting Classifier
Model Evaluation:
= Split the data into training and testing sets (70%/30%).
- Evaluated models using ROC AUC scores, confusion matrices, and classification reports.
- Gradient Boosting demonstrated strong predictive performance, with feature importance analysis conducted to identify the most influential predictors.
  
## 5. Key Findings
- Identified significant features affecting loan defaults (e.g., interest rates, employment length, and loan intent).
- High-risk loans, determined by interest rate, had a markedly higher likelihood of default.
- The relationship between customer demographics, homeownership, and default risk was visualized and quantified.

## Technologies and Tools
Languages: Python
Libraries:
- Data Manipulation: pandas, numpy
- Visualization: matplotlib, seaborn
Machine Learning: scikit-learn
Environment: Google Colab
## Instructions for Reproducing the Analysis
Clone the repository.
Place the dataset (credit_risk.csv) in the root folder.
Run the Google Colab to execute the analysis step-by-step.
Optional: Modify parameters or extend the analysis to include additional features/models.

## Next Steps
Explore advanced techniques like hyperparameter tuning to improve model performance.
Integrate additional datasets for broader insights.
Deploy the model into a production environment for real-time predictions.
