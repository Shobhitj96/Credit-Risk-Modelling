# Credit-Risk-Modelling

This project focuses on building a Credit Risk Model to assess the risk of loan approval using various statistical and machine learning techniques. The goal is to help financial institutions manage risk by categorizing customers into different risk profiles.

**Overview**

Credit risk modeling is crucial in the banking and finance sectors for assessing the likelihood of default. This project applies various statistical tests, feature selection techniques, and machine learning models to build an accurate classification model for loan approval risk.

**Project Objectives**

1. Build a robust model for classifying loan applicants based on risk.

2. Apply various preprocessing steps to prepare the data.
  
3. Use multiple algorithms to identify the best-performing model for accuracy and interoperability.

4. 
To ensure high-quality data, several preprocessing steps were implemented:

Handling Missing Values: Removed null values to ensure data consistency.

Data Merging: Combined datasets to include all relevant features.

**Statistical Test**

**Chi-Square Test**: Identified important categorical features related to the Approved_Flag by calculating p-values for categories like marital status, education, and gender.

**Multicollinearity Check**: Applied Variance Inflation Factor (VIF) to ensure low multicollinearity in numerical features.

**ANOVA Test**: Selected significant numerical features by evaluating F-statistics for features against loan approval categories.

**One-Hot Encoding**: Encoded categorical variables for model compatibility.


**Modeling Techniques**

The following models were trained and evaluated:

**Random Forest Classifier**

Accuracy: 0.764

Class Performance:

Class P1: Precision 0.84, Recall 0.70, F1 Score 0.76

Class P2: Precision 0.80, Recall 0.93, F1 Score 0.86

Class P3: Precision 0.44, Recall 0.21, F1 Score 0.29

Class P4: Precision 0.72, Recall 0.73, F1 Score 0.72

**XGBoost Classifier**

Accuracy: 0.78

Class Performance:

Class P1: Precision 0.82, Recall 0.76, F1 Score 0.79

Class P2: Precision 0.83, Recall 0.91, F1 Score 0.87

Class P3: Precision 0.48, Recall 0.31, F1 Score 0.37

Class P4: Precision 0.73, Recall 0.74, F1 Score 0.73

**Decision Tree Classifier**

Accuracy: 0.71

Class Performance:

Class P1: Precision 0.73, Recall 0.72, F1 Score 0.73

Class P2: Precision 0.81, Recall 0.83, F1 Score 0.82

Class P3: Precision 0.34, Recall 0.33, F1 Score 0.33

Class P4: Precision 0.65, Recall 0.63, F1 Score 0.64

**Hyperparameter Tuning with XGBoost**
Extensive hyperparameter tuning was conducted with XGBoost, achieving optimal results with:

learning_rate: 0.2

max_depth: 3

n_estimators: 200

Best Test Accuracy: 0.78

**Evaluation Metrics**

The model performance was evaluated using the following metrics:

Accuracy: Percentage of correctly predicted instances.

Precision, Recall, and F1 Score for each class (P1, P2, P3, P4) to assess class-wise performance.

**Technologies Used**

Python: for data manipulation and model building

Pandas: for data preprocessing

SciPy: for statistical tests

Scikit-Learn: for model training and evaluation

XGBoost: for optimized tree-based model

Flask: for web application deployment

**Results**
The XGBoost model achieved the highest accuracy of 78% on the test dataset, with fine-tuned hyperparameters providing an optimal balance between recall and precision.

**Future Improvements**
1.Experiment with ensemble models to improve predictive accuracy.

2.Refine feature engineering, particularly for numerical features.

3.Optimize the Flask app UI for ease of use.
