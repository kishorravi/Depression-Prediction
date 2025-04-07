# 🎓 Student Depression Detection using Machine Learning

This project aims to analyze and predict depression among students based on various academic, demographic, and lifestyle factors using machine learning. It uses a real-world dataset of students with features such as academic pressure, CGPA, sleep duration, dietary habits, and more.

---

## 📁 Dataset

**Source**: [Student Depression Dataset: Analyzing Mental Health Trends and Predictors Among Students](https://www.kaggle.com/datasets/adilshamim8/student-depression-dataset)

The dataset includes:
- Demographics (Gender, Age, City)
- Academic indicators (CGPA, Academic Pressure)
- Lifestyle & wellbeing (Sleep Duration, Work Pressure, Dietary Habits)
- Psychological indicators (Suicidal Thoughts, Family History)
- **Target**: Depression (Yes/No)

---

## 📊 Features Used

- Gender  
- Age  
- City  
- Profession  
- CGPA  
- Academic Pressure  
- Work Pressure  
- Study Satisfaction  
- Job Satisfaction  
- Sleep Duration  
- Dietary Habits  
- Degree  
- Suicidal Thoughts  
- Work/Study Hours  
- Financial Stress  
- Family History of Mental Illness  

---

## 🧠 Machine Learning Model

- **Model Used**: Random Forest Classifier  
- **Preprocessing**:
  - Label Encoding of categorical variables
  - Standardization using `StandardScaler`
- **Evaluation Metrics**:
  - Accuracy
  - Precision, Recall, F1-score
  - Confusion Matrix
- **Split**:
  - 64% Training
  - 16% Validation
  - 20% Testing

---

## 🛠️ How to Run

### 📦 Requirements

- Python 3.x
- Pandas, Numpy
- Scikit-learn
- Seaborn, Matplotlib
- Joblib

### ▶️ Run the notebook

1. Upload the dataset (`student_depression_dataset.csv`) to the working directory or Google Drive.
2. Open and run `Untitled.ipynb` or your main `.ipynb` file.
3. The model will:
   - Perform EDA
   - Train a classifier
   - Evaluate on validation and test sets
   - Save the trained model and scaler

---

## 📈 Results

- Achieved **high accuracy** on validation and test sets
- Top contributing features include:
  - CGPA
  - Academic Pressure
  - Sleep Duration
  - Suicidal Thoughts
  - Study Satisfaction

---

## 💾 Output

- `depression_model.pkl`: Trained Random Forest model
- `scaler.pkl`: StandardScaler instance

---

## 📄 License

Licensed under [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0).

---

## 🙏 Acknowledgements

Thanks to the Kaggle contributor for providing a clean and rich dataset.

---

## 🤝 Contributing

Pull requests are welcome. For major changes, please open an issue first.

---

## 💬 Contact

For queries, feel free to contact [Your Name] at [Your Email or LinkedIn]
