# 📊 Predicting Student Depression Using Machine Learning on Lifestyle and Academic Indicators

This project uses machine learning to predict depression among students based on their academic performance, lifestyle choices, and psychological indicators. The goal is to identify key predictors of depression and build a model that helps in early detection and potential intervention.

---

## 📁 Dataset

- **Name**: Student Depression Dataset
- **Source**: [Kaggle - Student Depression Dataset](https://www.kaggle.com/datasets/adilshamim8/student-depression-dataset)
- **Size**: ~28,000 records
- **Format**: CSV
- **Target Variable**: `Depression` (Yes/No or 1/0)

---

## 🧠 Features Included

- **Demographics**: Gender, Age, City, Profession
- **Academics**: CGPA, Academic Pressure, Degree, Study Satisfaction
- **Work-Life Balance**: Work Pressure, Job Satisfaction, Work/Study Hours
- **Lifestyle & Mental Health**: Sleep Duration, Dietary Habits, Financial Stress, Suicidal Thoughts, Family History of Mental Illness

---

## 📊 Exploratory Data Analysis

### 📌 Distribution of CGPA
![CGPA Distribution](images/Unknown-4.png)

### 📌 CGPA vs Depression
![CGPA vs Depression](images/Unknown-5.png)

### 📌 Correlation Heatmap
![Correlation Heatmap](images/Unknown-6.png)

### 📌 Feature Importance from Random Forest
![Feature Importance](images/Unknown-7.png)

---

## 🛠️ Model Pipeline

- **Model Used**: Random Forest Classifier
- **Preprocessing**:
  - Categorical variables encoded using `LabelEncoder`
  - Standardized using `StandardScaler`
- **Split**:
  - 64% Training
  - 16% Validation
  - 20% Testing

---

## 🧪 Results

- **Validation Accuracy**: ~XX.XX%
- **Test Accuracy**: ~XX.XX%
- **Top Features Influencing Depression**:
  1. Have you ever had suicidal thoughts?
  2. Academic Pressure
  3. Financial Stress
  4. CGPA
  5. Sleep Duration

---

## 💾 Output Files

- `depression_model.pkl` – Trained Random Forest model
- `scaler.pkl` – Scaler used for input normalization
- `Student_Depression_Predictor.ipynb` – Complete notebook with EDA, preprocessing, and model

---

## 🚀 Usage

### 1. Clone this repository

```bash
git clone https://github.com/your-username/student-depression-prediction.git
cd student-depression-prediction
s
