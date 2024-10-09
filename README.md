# Customer_curn_project

Churn Prediction using Logistic Regression and Decision Tree
This project is focused on predicting customer churn for an e-commerce company using two classification models: Logistic Regression and Decision Tree. The dataset includes various customer features, and the target is to predict whether a customer will churn (leave) or stay.

Project Overview
The main objectives of this project are:

Data Preprocessing: Handle missing data, standardize features, and convert categorical variables into numerical format.
Visualization: Plot histograms, count plots, and other visualizations to understand the data distribution and relationships.
Modeling: Train and evaluate two machine learning models – Logistic Regression and Decision Tree.
Model Evaluation: Use confusion matrix, ROC curve, and classification reports to assess model performance.
Dataset
The dataset is an e-commerce dataset with 20 features and includes information such as:

CustomerID: Unique ID of the customer.
Churn: Target variable indicating whether the customer churned (1) or not (0).
Tenure: Duration (in months) the customer has been with the organization.
PreferredLoginDevice: Device the customer uses to log in.
CityTier: Tier of the city the customer belongs to.
WarehouseToHome: Distance between the customer’s home and the warehouse.
PreferredPaymentMode: Preferred payment method of the customer.
Gender: Gender of the customer.
OrderCount: Total number of orders placed by the customer.
CashbackAmount: Cashback amount earned by the customer.
You can find the dataset at the following URL:

Dataset URL
Steps and Workflow
1. Data Preprocessing
Load the dataset using Pandas.
Handle missing values by removing rows with NaN values.
Encode categorical columns such as MaritalStatus and Gender using pd.get_dummies.
Standardize numerical columns using StandardScaler.
2. Data Visualization
Visualize the distribution of key features such as Tenure, OrderCount, and CashbackAmount.
Explore the churn rate among customers based on categorical features such as Gender and MaritalStatus.
Use histograms and count plots for better understanding of data distribution.
3. Model Training and Evaluation
Logistic Regression Model:
Train a Logistic Regression model and evaluate its performance using classification reports, confusion matrix, and ROC curve.
Display the model's accuracy score.
Decision Tree Model:
Train a Decision Tree model and evaluate its performance using the same metrics.
Visualize the decision tree’s accuracy, confusion matrix, and ROC curve.
4. Performance Metrics
Confusion Matrix: Displays true positives, true negatives, false positives, and false negatives.
ROC Curve: Shows the trade-off between sensitivity and specificity.
Classification Report: Provides precision, recall, F1-score, and support for both classes.
Requirements
To run this project, you need the following Python libraries:

bash
Copy code
pip install pandas numpy scikit-learn seaborn matplotlib
Running the Project
Clone the repository or download the script.
Make sure you have the necessary libraries installed (use the requirements mentioned above).
Load the dataset using the provided URL or a local copy.
Run the script to preprocess the data, train the models, and evaluate their performance.
bash
Copy code
python churn_prediction.py
Output Example
After running the script, you will get output similar to the following:

bash
Copy code
              precision    recall  f1-score   support

           0       0.89      0.98      0.93       849
           1       0.75      0.38      0.50       163

    accuracy                           0.88      1012
   macro avg       0.82      0.68      0.72      1012
weighted avg       0.87      0.88      0.86      1012

Model aniqligi: 0.8794
In addition to classification reports, confusion matrices, and ROC curves will be displayed as visualizations.
