# 🎓 Predicting Student Depression Using Machine Learning on Academic, Lifestyle & Mental Health Indicators

This project investigates the prediction of depression among students using machine learning. It leverages a large dataset of student-related features — including academic metrics, lifestyle habits, and psychological indicators — to identify factors influencing depression and build a predictive model.

---

## 📁 Dataset Overview

- **Name**: Student Depression Dataset
- **Source**: [Kaggle](https://www.kaggle.com/datasets/adilshamim8/student-depression-dataset)
- **Records**: ~27,900 student profiles
- **Format**: CSV
- **Target Variable**: `Depression` (binary: Yes/No or 1/0)

### 🔍 Features Included

| Category | Features |
|----------|----------|
| Demographics | Gender, Age, City, Profession |
| Academic | CGPA, Academic Pressure, Study Satisfaction, Degree |
| Workload | Work Pressure, Job Satisfaction, Work/Study Hours |
| Wellbeing | Sleep Duration, Dietary Habits, Financial Stress |
| Mental Health | Suicidal Thoughts, Family History of Mental Illness |

---

## 🧠 Project Goals

- Analyze mental health trends among students using data
- Visualize correlations and contributing factors
- Build a predictive model using Random Forest
- Identify top features influencing depression
- Help design early intervention strategies

---

## 🔍 Exploratory Data Analysis (EDA)

### 📊 CGPA Distribution

A right-skewed distribution shows most students have a CGPA between 6 and 9.  
This indicates good academic standing for the majority, but even students with higher CGPA may suffer from depression.

![Distribution of CGPA](https://github.com/kishorravi/Depression-Prediction/blob/main/Unknown-4.png)

---

### 📉 CGPA vs Depression

Interestingly, there’s no sharp decline in CGPA for students with depression, which suggests **academic performance alone isn't a strong predictor** of depression.

![CGPA vs Depression](https://github.com/kishorravi/Depression-Prediction/blob/main/Unknown-5.png)

---

### 🧬 Correlation Heatmap

This heatmap shows correlations between various features.  
Key observations:
- Depression has strong positive correlation with **Suicidal Thoughts**, **Academic Pressure**, and **Financial Stress**.
- CGPA shows almost **no correlation** with Depression.

![Correlation Heatmap](https://github.com/kishorravi/Depression-Prediction/blob/main/Unknown-6.png)

---

### 💡 Feature Importance

Feature importances from the Random Forest model reveal that **suicidal thoughts**, **academic pressure**, and **financial stress** are the most influential factors in predicting depression.

![Feature Importance](https://github.com/kishorravi/Depression-Prediction/blob/main/Unknown-7.png)

---

## 🛠️ Model Pipeline

- **Algorithm**: Random Forest Classifier
- **Preprocessing**:
  - Label Encoding for categorical variables
  - StandardScaler for numerical features
- **Data Split**:
  - 64% Training
  - 16% Validation
  - 20% Testing
- **Evaluation**:
  - Accuracy, Precision, Recall, F1-Score, Confusion Matrix

---

## ✅ Model Results

### 📊 Validation Set
- Accuracy: **84.9%**
- Precision (Depressed): 86%
- Recall (Depressed): 88%
- F1 Score: 87%

### 🧪 Test Set
- Accuracy: **82.7%**
- Precision (Depressed): 84%
- Recall (Depressed): 87%
- F1 Score: 85%

> The model shows strong generalization with high performance on both validation and test sets. It is especially effective at identifying students who are at risk of depression (high recall for class 1). This ensures that fewer at-risk students go unnoticed.
> **Top Features**:
> 1. Suicidal Thoughts  
> 2. Academic Pressure  
> 3. Financial Stress  
> 4. Work/Study Hours  
> 5. CGPA

---

## 📂 Output Files

- `Student_Depression_Predictor.ipynb` – Full code and EDA
- `depression_model.pkl` – Trained Random Forest model
- `scaler.pkl` – StandardScaler used during preprocessing

---

## 🧪 Run It Yourself

### 1. Clone this repository
```bash
git clone https://github.com/kishorravi/Depression-Prediction.git
cd Depression-Prediction
