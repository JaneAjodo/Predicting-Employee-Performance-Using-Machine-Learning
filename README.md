# 🧠 Employee Performance Classification with Machine Learning

This project aims to predict employee performance levels (Low, Average, High) using machine learning techniques.


## 📊 Dataset

- Sourced from a public HR dataset on [Kaggle](https://www.kaggle.com/datasets/nadeemajeedch/employee-performance-and-salary-dataset)
- ~500 records with attributes like:
  - Age, Gender, Department, Status
  - Salary, Experience, Session
  - Tenure (from Joining Date)
  - Performance Score (Target variable)


## 🧹 Data Preprocessing

- Removed records with missing target values
- Created `Tenure (Years)` from `Joining Date`
- Mapped performance scores to 3 classes:
  - 1–2 → Low, 3 → Average, 4–5 → High
- Label encoded categorical variables
- Standardized numerical features

## 🤖 Models Used

- Logistic Regression  
- Random Forest  
- XGBoost (Best performing model)


## 📈 Results

| Model                | Accuracy | F1 Score |
|----------------------|----------|----------|
| ✅ XGBoost            | 50.5%    | 50.5%    |
| Random Forest        | 49.5%    | 48.3%    |
| Logistic Regression  | 44.6%    | 40.0%    |

**Top 10 Important Features:**
`Status`, `Age`, `Session`, `Experience`, `Salary`, `Tenure`, `Department`, `Gender`, `Location`

## 📌 Future Improvements

- Hyperparameter tuning (e.g. GridSearchCV)
- Class imbalance handling (SMOTE, class weights)
- Deep Learning with MLPs
- Expand dataset or simulate more data

## 📎 Links

- 📘 [Full Medium Article](https://medium.com/@janeajodo/predicting-employee-performance-using-machine-learning-a220cc013ff4)

## 🛠️ Tools & Tech

- Python (pandas, scikit-learn, XGBoost)
- Jupyter Notebook
- Matplotlib/Seaborn for visualizations
