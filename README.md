# Credit Risk Analysis and Modeling
Stalog (German Credit Data)
# Busniness Understanding 
It contains data on 1,000 loan applicants from a German bank, and the objective is to predict whether an applicant is a good or bad credit risk based on various attributes such as their credit history, employment status, and personal information.
# Data Understanding
The dataset has 9 input attributes such as credit history, purpose of the loan, personal status and sex, property status and housing type, employment status, age, and others, and one target attribute which is binary indicating whether the credit risk is good or bad.
# Data Preparation
The process of preparing the data for credit analysis involved several important steps. First, the missing values ​​in the columns 'Savings Account' and 'Checking Account' were handled by assigning them a value of 0 and labeling them using the SC_LabelEncoder function. Similarly, the column 'Housing' was label-encoded using the Housing_LabelEncoder function. Next, the categorical variables such as 'Gender', 'Purpose' and 'Risk' were converted to numeric form using LabelEncoder from scikit-learn. Finally, the dataset was split into a training set and a test set using the train_test_split function to prepare for model building.
# Modeling
After data preparation, several classification models were evaluated using the 5-fold cross-validation method, including Logistic Regression, Support Vector Machine (SVC), Decision Tree, Random Forest, and Gaussian naive Bayes. Random Forest achieved the best performance on both the training and testing sets.To address the imbalanced data, the SMOTE oversampling technique was applied to create a more balanced dataset. 

Random Forest Classifier Results:

+ Attained 79% accuracy on the test data.

XGBOOST Results:

+ Attained 79% accuracy on the test data

The confusion matrix found the model to have good classification ability for both customer groups, with the expected number of mismatches. The ROC curve also showed that the area under the curve (AUC) reached 0.97, demonstrating the model has high analytical ability between the two risk groups.
# Conclusion on Modeling:
Both RandomForestClassifier and XGBoost show a good balance in identifying good and bad credit. Visualizations such as confusion matrix and ROC curve highlight areas for improvement in credit scoring reliability and robustness.
