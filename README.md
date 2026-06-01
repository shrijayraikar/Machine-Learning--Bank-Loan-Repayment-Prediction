# Machine-Learning--Bank-Loan-Repayment-Prediction
This project applies supervised machine learning to predict whether a bank loan applicant will repay their loan or default.

**Dataset & Features**

The model is trained on historical loan data (Loan_Repayment_Training_Data.csv) containing applicant attributes such as Employment Status, Marital Status, and Education Level. The target variable is binary: Repay (1) or Default (0).

**Preprocessing**

Categorical features (Employment Status, Marital Status, Education Level) are converted into numerical format using one-hot encoding (pd.get_dummies), making them suitable for the algorithm.

**Model**

A Logistic Regression classifier from scikit-learn is used — a well-suited algorithm for binary classification problems. The data is split 80/20 into training and test sets, the model is fitted on the training data, and accuracy is evaluated on the held-out test set.

**Prediction**

Once trained, the model is applied to a new, unlabeled dataset (Loan_Repayment_Test_Data_NoLabel.csv) to generate predictions. Results are decoded back to human-readable labels ("Repay" / "Default") and exported to an Excel file (Bank_Loan_Predictive_Data.xlsx) for reporting.

**In summary**, this is a straightforward yet practical binary classification pipeline that helps banks automate loan risk assessment, reducing manual effort while providing data-driven repayment predictions.
