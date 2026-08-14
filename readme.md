# Student Performance Predictor

A machine learning project that predicts students' final scores using academic, behavioral, and demographic features.

## 📌 Project Overview

The goal of this project is to build a regression model that can predict a student's `final_score` based on information such as study hours, previous performance, attendance, assignments, internet usage, and sleep.

The project follows a complete machine learning workflow:

**Data Understanding → EDA → Data Cleaning → Feature Engineering → Preprocessing → Model Training → Evaluation → Feature Importance → Overfitting Analysis → Basic Model Tuning**

## 📊 Dataset

The dataset contains student-related information including:

* Study hours
* Previous score
* Attendance percentage
* Assignments completed
* Internet usage
* Sleep hours
* Gender
* Parent education
* Internet access
* Study method
* Other student-related features

The target variable is:

`final_score`

## 🔎 Exploratory Data Analysis

EDA was performed to understand:

* Feature distributions
* Relationships between individual features and final score
* Categorical feature differences
* Correlations between numerical variables
* Potential patterns and outliers

## 🧹 Data Cleaning & Preprocessing

The project includes:

* Checking for duplicate records
* Handling missing values
* Cleaning inconsistent categorical values
* Converting percentage values into numerical form
* Removing rows with missing target values
* One-hot encoding categorical variables
* Separating features and target
* Train-test splitting

## 🤖 Models Used

### Linear Regression

Used as a simple baseline regression model.

### Random Forest Regressor

Used to capture more complex and non-linear relationships between the features and final score.

A basic tuning step was also performed on the Random Forest to reduce overfitting.

## 📈 Model Evaluation

The models were evaluated using:

* **MAE (Mean Absolute Error)** — lower is better
* **RMSE (Root Mean Squared Error)** — lower is better
* **R² (R-squared)** — higher is better

### Final Model Performance

The tuned Random Forest achieved approximately:

| Metric | Score |
| ------ | ----: |
| R²     | 0.479 |
| MAE    | 2.236 |
| RMSE   | 4.014 |

The Random Forest performed better than the Linear Regression baseline on the test set.

## 🔍 Feature Importance

Feature importance from the Random Forest showed that features such as:

* `study_hours`
* `previous_score`
* `attendance_percent`
* `assignments_completed`
* `internet_hours`
* `sleep_hours`

provided the strongest predictive signal among the features used by the model.

Feature importance represents predictive importance within the model and should not be interpreted as causation.

## 📉 Overfitting Analysis

Training and testing performance were compared to identify overfitting.

The initial Random Forest showed a significant difference between training and testing R², indicating overfitting. Basic model constraints were then applied to reduce model complexity and improve generalization.

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Jupyter Notebook

## 📁 Project Structure

```text
student-performance-predictor/
│
├── student_performance_predictor.ipynb
├── README.md
└── dataset/
    └── student_performance.csv
```

## 🚀 How to Run

1. Clone the repository.
2. Install the required Python libraries.
3. Open `student_performance_predictor.ipynb` in Jupyter Notebook or JupyterLab.
4. Run the notebook cells from top to bottom.

## 🎯 Key Learning Outcomes

Through this project, I practiced:

* Exploratory Data Analysis
* Data cleaning
* Missing value handling
* Feature engineering
* Categorical encoding
* Train-test splitting
* Regression modeling
* Model evaluation
* Feature importance
* Identifying and reducing overfitting

## 👤 Author

**Pranav Sharma**

