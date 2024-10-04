# Customer Churn Prediction

This project is focused on predicting customer churn for a subscription-based U.S. bank service. The model uses historical customer data including demographics, usage behavior, and account information to predict whether a customer will leave the bank.

## Project Overview

The dataset contains customer details like age, credit score, gender, tenure, balance, and the number of products used, among others. The target variable is `Exited`, which indicates if a customer has churned (`1`) or not (`0`).

### Features

- **CreditScore**: Customer's credit score.
- **Geography**: The country of the customer (France, Germany, or Spain).
- **Gender**: Customer's gender (Male or Female).
- **Age**: Customer's age.
- **Tenure**: Number of years the customer has been with the bank.
- **Balance**: The account balance of the customer.
- **NumOfProducts**: Number of bank products the customer is using.
- **HasCrCard**: Does the customer have a credit card?
- **IsActiveMember**: Is the customer an active member?
- **EstimatedSalary**: Customer's estimated salary.
- **Exited**: Churn label (1 = Yes, 0 = No).

### Libraries Used

- Python 3.x
- NumPy
- pandas
- scikit-learn
- matplotlib
- seaborn

### Models Used

1. **Logistic Regression**
2. **Random Forest Classifier**
3. **Gradient Boosting Classifier**

### Evaluation Metrics

- **Accuracy**: The overall performance of the model.
- **Confusion Matrix**: A summary of prediction results.
- **ROC Curve**: A graphical plot to illustrate the performance of the binary classification models.

## Installation and Setup

1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/customer-churn-prediction.git
    cd customer-churn-prediction
    ```

2. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. Run the `churn_prediction.py` file to train models and visualize the results.

## Usage

1. **Data Preprocessing**: The categorical variables (like Geography and Gender) are encoded, and the numerical features are scaled.
2. **Model Training**: The data is split into training and testing sets. Three models are trained for comparison.
3. **Model Evaluation**: Accuracy, confusion matrix, and ROC curves are used to evaluate the models.
4. **Visualization**: Various data exploration and model performance plots (correlation heatmap, churn distribution, ROC curve, and feature importance).

## Visualizations

-**Correlation Matrix Heatmap**: Shows relationships between features.
- **Churn Distribution**: Visualizes churn vs non-churned customers.
- **Churn by Geography**: Displays churn rate based on geography.
- **ROC Curve**: Compares the performance of different models.
- **Feature Importance**: Visualizes the important features in the Random Forest model.

## Conclusion

The project compares the performance of multiple machine learning algorithms for churn prediction, with Random Forest and Gradient Boosting providing higher accuracy and better predictive power compared to Logistic Regression.

