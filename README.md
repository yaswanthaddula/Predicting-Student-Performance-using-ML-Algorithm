# 🎓 Predicting Student Academic Performance using Linear Regression

## ▶️ Clone the Repository

git clone https://github.com/yaswanthaddula/Predicting-Student-Performance-using-ML-Algorithm  
cd Predicting-Student-Performance-using-ML-Algorithm  

---

## 📌 Project Overview

This project predicts student academic performance using Linear Regression. The system takes academic and behavioral inputs from students and predicts their final exam score. Based on the predicted score, the system assigns a grade, determines pass or fail status, and identifies whether the student is at academic risk.

The goal of this project is to build a data-driven model that helps institutions identify performance trends and detect students who may need academic support.

---

## 📂 Dataset Description

The dataset contains the following input features:

- Hours_Studied (0–24)
- Attendance (0–100)
- Previous_Scores (0–100)
- Tutoring_Sessions (0–10)
- Sleep_Hours (0–12)
- Teacher_Quality (Low / Medium / High)
- School_Type (Public / Private)
- Parental_Education_Level (High School / College / Postgraduate)

Target Variable:
- Exam_Score

---

## 🔄 Data Preprocessing

Before training the model:

- Checked for missing values
- Filled missing categorical values using mode
- Converted categorical values into numeric format:
  - Teacher_Quality → Low=1, Medium=2, High=3
  - School_Type → Public=0, Private=1
  - Parental_Education_Level → High School=1, College=2, Postgraduate=3
- Split dataset into 80% training and 20% testing data

---

## 🤖 Machine Learning Model

Linear Regression from Scikit-learn is used to predict continuous exam scores. The model learns the relationship between input features and the target variable using a best-fit linear equation.

---

## 📊 Model Evaluation Results

R² Score: 0.658  
Mean Squared Error (MSE): 4.839  
Root Mean Squared Error (RMSE): 2.2  

Interpretation:

- The model explains approximately 65.8% of the variation in exam scores.
- On average, predictions are off by about 2.2 marks.

---

## 📈 Example Prediction

Input Provided:

Hours Studied: 23  
Attendance: 84  
Previous Score: 73  
Tutoring Sessions: 0  
Sleep Hours: 7  
Teacher Quality: Medium  
School Type: Public  
Parental Education Level: High School  

Output Generated:

Predicted Exam Score: 67.65  
Result: Pass  
Grade: D  
At Risk: No  

---

## 🎯 Output Logic

Grade Classification:

- 90 and above → Grade A  
- 80–89 → Grade B  
- 70–79 → Grade C  
- 60–69 → Grade D  
- Below 60 → Grade F  

Pass/Fail Logic:

- Marks ≥ 40 → Pass  
- Marks < 40 → Fail  

Risk Detection Logic:

A student is considered "At Risk" if:
- Predicted Score < 50  
OR  
- Attendance < 60  
OR  
- Previous Score < 50  

---

## 🛠 Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib

---

## ▶️ How to Run

Install required libraries:

pip install pandas numpy scikit-learn matplotlib  

Run the project:

python main.py  

Enter student details when prompted to receive predicted results.

---

## 🚨 Limitations

- The model assumes a linear relationship between features and exam score.
- Performance depends on dataset quality and size.
- The model may not generalize to different institutions without retraining.

---

## 🔮 Future Improvements

- Apply Polynomial Regression for non-linear relationships
- Use Random Forest Regressor for improved performance
- Apply Cross-Validation
- Deploy as a web-based application

---

## 👤 Author

Yaswanth Addula  
B.Tech – Computer Science / Data Science
