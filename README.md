# Student Performance Prediction using Machine Learning

## 📌 Project Overview

This project uses Machine Learning to predict students' final scores based on their study hours and attendance.

A Multiple Linear Regression model was trained and evaluated using a student performance dataset containing 20 students.

The project demonstrates the complete Machine Learning workflow, including:

- Data loading and exploration
- Data cleaning
- Correlation analysis
- Linear Regression
- Multiple Linear Regression
- Train/Test Split
- Model Prediction
- Model Evaluation
- Data Visualization

---

## 🎯 Objective

The main objective of this project is to analyze how study hours and attendance affect students' final scores and build a Machine Learning model that can predict the final score of a student.

---

## 📊 Dataset Information

The dataset contains information about 20 students.

### Features

| Feature | Description |
|---|---|
| `student_id` | Unique ID of each student |
| `study_hours` | Number of hours studied |
| `attendance` | Student attendance percentage |
| `previous_score` | Previous academic score |
| `sleep_hours` | Average sleeping hours |
| `extracurricular` | Participation in extracurricular activities |
| `final_score` | Final academic score |

### Dataset Shape

```text
(20, 7)

Missing Values
There were no missing values in the dataset.
All columns: 0 missing values

🔍 Data Analysis
Correlation analysis was performed to understand the relationship between different features and the final score.
Study Hours vs Final Score
Correlation: 0.98
This shows a strong positive relationship between study hours and final score.

Attendance vs Final Score
Correlation: 0.98
This also shows a strong positive relationship between attendance and final score.

🤖 Machine Learning Model
Two regression approaches were explored:
1. Single Linear Regression
The first model used:
Study Hours
to predict the final score.
The model achieved:
R² Score: 0.97

2. Multiple Linear Regression
The final model used two features:
Study Hours
Attendance
The model was trained using an 80/20 train-test split.
Training Data: 16 students
Testing Data: 4 students

📈 Model Evaluation
The final Multiple Linear Regression model was evaluated using the test dataset.
Results
Metric	Result
Test R² Score	0.97
Mean Absolute Error (MAE)	1.87
Root Mean Squared Error (RMSE)	2.09

Interpretation
R² Score = 0.97 indicates that the model explains a large proportion of the variation in the test scores.
MAE = 1.87 means the model's predictions were off by about 1.87 marks on average.
RMSE = 2.09 indicates the typical prediction error while giving more weight to larger errors.

🧮 Model Equation
The trained Multiple Linear Regression model produced the following approximate equation:
Predicted Score = 11.76
                  + (3.31 × Study Hours)
                  + (0.62 × Attendance)
This means that, within this model and dataset:
Study hours have a positive relationship with predicted score.
Attendance also has a positive relationship with predicted score.

🎓 Example Prediction

A new student with:
Study Hours = 8
Attendance = 95%
was given to the trained model.
Predicted Final Score
96.74

📊 Visualizations

The project includes visualizations for:
Actual vs Predicted Final Scores
Test Data Actual vs Predicted Scores
Actual vs Predicted Score Scatter Plot
Model performance comparison
These visualizations help understand how closely the model predictions match the actual scores.

🔎 Project Findings
Study hours showed a strong positive relationship with final scores.
Attendance also showed a strong positive relationship with final scores.
Multiple Linear Regression achieved a Test R² Score of 0.97.
The average prediction error was 1.87 marks.
The RMSE was 2.09 marks.
A student with 8 study hours and 95% attendance was predicted to score 96.74.

🛠️ Technologies Used
Python
Google Colab
Pandas
NumPy
Matplotlib
Scikit-learn
GitHub

📚 Machine Learning Workflow
Dataset
   ↓
Data Exploration
   ↓
Data Cleaning
   ↓
Correlation Analysis
   ↓
Linear Regression
   ↓
Multiple Linear Regression
   ↓
Train/Test Split
   ↓
Model Training
   ↓
Prediction
   ↓
Model Evaluation
   ↓
Visualization

🚀 Future Improvements
This project can be improved by:
Increasing the dataset size
Using all available relevant features
Comparing different Machine Learning algorithms
Performing cross-validation
Hyperparameter tuning
Adding more student performance features
Deploying the model as a web application

👨‍💻 Author
Muhammad Usman
This project was created as a Machine Learning portfolio project to demonstrate data analysis, regression modeling, prediction, and model evaluation using Python.

⭐ Project Conclusion

This project demonstrates how Machine Learning can be used to analyze student performance and predict final scores using study hours and attendance.
The Multiple Linear Regression model achieved a 0.97 Test R² Score, with an MAE of 1.87 and RMSE of 2.09 on the test dataset.
