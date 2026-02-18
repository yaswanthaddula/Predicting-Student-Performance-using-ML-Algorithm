## 🎓 Student Performance Classification Using Logistic Regression
📌 Project Overview
This project uses Logistic Regression to classify students based on academic and behavioral factors.

Instead of predicting exact marks, the model predicts:

Pass / Fail
At Risk / Not At Risk
The objective is to identify students who may need academic support early.

🎯 Problem Statement
Educational institutions often lack predictive systems to detect academic risk in advance.
This project builds a classification model to:
Predict whether a student will pass or fail
Identify students at academic risk

Support early intervention strategies

📂 Dataset Features
The dataset includes:

Hours Studied (0–24)
Attendance Percentage (0–100)
Previous Exam Score (0–100)
Tutoring Sessions (0–10)
Sleep Hours (0–12)
Teacher Quality (Low/Medium/High)
School Type (Private/Public)
Parental Education Level (High School/College/Postgraduate)
Final Result (Pass = 1, Fail = 0)
Categorical features were encoded before training.

🛠 Technologies Used
Python
NumPy
Pandas
Matplotlib

Scikit-learn

🤖 Model Used
Logistic Regression
Logistic Regression is a supervised classification algorithm that estimates the probability of a binary outcome using the sigmoid function.

It outputs:
Probability of passing
Class label (Pass or Fail)

📊 Model Evaluation Metrics
Since this is classification, we evaluate using:

Accuracy
Precision
Recall
F1-Score

Example (replace with your actual results):

Accuracy: 87%
Precision: 85%
Recall: 82%
F1 Score: 83%

If your accuracy is below 65%, your model is weak. Be honest.

🔄 Data Preprocessing
Removed missing values (NaN handling)
Encoded categorical variables using Label Encoding / One-Hot Encoding
Feature scaling applied (StandardScaler)
Train-Test Split (e.g., 80% train, 20% test)

