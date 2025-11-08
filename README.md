## End to End ML Project

# 🎓 Student Performance Prediction — End-to-End Machine Learning Project  

### *Predicting student academic outcomes using demographic and educational attributes*  

---

## 📘 Overview  

This project implements an **end-to-end machine learning pipeline** to analyze and predict **student performance** based on social and educational factors such as gender, parental education, lunch type, and test preparation course.  

It demonstrates every step of a real-world ML workflow — **data collection, exploration, model building, evaluation, and web deployment** using Flask.  

---

## 🎯 Objective  

To build a **regression model** that predicts a student’s **average test score** (based on math, reading, and writing scores) using input variables such as gender, race/ethnicity, and parental education level.  

This helps identify factors that most influence student success and can be used to guide educational interventions.  

---

## 🗂️ Project Structure  

```bash
ml_practice_project/
│
├── .vscode/
│   └── settings.json            # VS Code workspace settings
│
├── data/
│   └── stud.csv                 # Student performance dataset
│
├── notebook/                    # Jupyter notebooks for exploration & experiments
│   ├── 1. EDA STUDENT PERFORMANCE.ipynb
│   └── 2. MODEL TRAINING.ipynb
│
├── src/
│   ├── components/              # Data ingestion, transformation, model training modules
│   ├── pipeline/                # Training & prediction pipeline scripts
│   ├── exception.py             # Custom exception handling
│   ├── logger.py                # Logging configuration
│   ├── utils.py                 # Helper functions
│   └── __init__.py
│
├── templates/                   # HTML templates for Flask app
│   ├── home.html
│   └── index.html
│
├── catboost_info/               # CatBoost logs folder
│
├── app.py                       # Flask application
├── requirements.txt              # Python dependencies
├── README.md                    # Project documentation
└── .gitignore                   # Git ignore file

## 🧠 Dataset Description  

The dataset `stud.csv` contains details about students’ demographic background and test scores in three subjects.  

| Feature | Description |
|----------|-------------|
| `gender` | Student gender (male/female) |
| `race_ethnicity` | Group category (A, B, C, D, E) |
| `parental_level_of_education` | Highest education level attained by a parent |
| `lunch` | Type of lunch received (standard/free-reduced) |
| `test_preparation_course` | Completion status of a test preparation course |
| `math_score` | Math score (0–100) |
| `reading_score` | Reading score (0–100) |
| `writing_score` | Writing score (0–100) |

The project may also use an engineered variable like:  
> **`average_score` = (math_score + reading_score + writing_score) / 3**

---

## 🧩 Features  

✅ **Exploratory Data Analysis (EDA)** — trends, distributions, and relationships between variables  
✅ **Feature Engineering** — transforming categorical and numerical variables  
✅ **Model Training** — regression models such as Linear Regression, Random Forest, CatBoost, etc.  
✅ **Model Evaluation** — metrics like R², RMSE, and MAE  
✅ **Flask Deployment** — interactive web app to input student details and predict scores  
✅ **Logging & Exception Handling** — for better debugging and traceability  

---

## 💡 Technology Stack  

| Category | Tools |
|-----------|-------|
| Programming Language | Python 3.x |
| Data Analysis | pandas, numpy |
| Machine Learning | scikit-learn, CatBoost, XGBoost |
| Visualization | matplotlib, seaborn |
| Deployment | Flask |
| IDE | VS Code / Jupyter Notebook |
| Version Control | Git & GitHub |

---

## ⚙️ Installation & Setup  

### 1️⃣ Clone the repository  
```bash
git clone https://github.com/aru2802/ml_practice_project.git
cd ml_practice_project
