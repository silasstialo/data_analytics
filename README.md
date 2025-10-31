# 🧠 Employment Suitability Prediction using Decision Tree

## 📘 Overview
This project applies a **Decision Tree Classification Model** to predict whether a job applicant is suitable for employment based on features such as age, education level, work experience, and assessment scores.  

It demonstrates a full **machine learning workflow** — from data loading and preprocessing to model building, visualization, and evaluation.

---

## 🧩 Dataset Description

Each record in the dataset represents a job applicant and contains the following features:

| Feature | Description |
|----------|-------------|
| `age` | Applicant’s age (in years) |
| `education_level` | Highest education attained (High School, Bachelor’s, Master’s, PhD) |
| `years_of_experience` | Total professional experience in years |
| `technical_test_score` | Score in technical test (out of 100) |
| `interview_score` | Score in interview (out of 10) |
| `previous_employment` | Previous job experience (Yes/No) |
| `suitable_for_employment` | Target variable (Yes/No) |

---

## ⚙️ Steps Performed

### 1️⃣ Data Loading and Exploration
- Loaded dataset using **pandas**.
- Displayed first few rows, checked datatypes, null values, and feature distributions.

### 2️⃣ Data Preprocessing
- Replaced missing numeric values with **mean/median**.
- Replaced missing categorical values with **‘unknown’**.
- Converted categorical features into numeric values using **label encoding**.
- Split data into **training (80%)** and **testing (20%)** subsets.

### 3️⃣ Model Building
- Trained a **DecisionTreeClassifier** from `sklearn` using training data.
- Target variable: `suitable_for_employment`.

### 4️⃣ Model Visualization
- Visualized the trained Decision Tree using `plot_tree()` from **matplotlib**.

### 5️⃣ Model Testing and Predictions
- Predicted employment suitability for test data.
- Tested model on a few **hypothetical candidate profiles** to interpret predictions.

### 6️⃣ Model Evaluation
- Evaluated the model using:
  - **Accuracy Score**
  - **Confusion Matrix** (visualized using Seaborn)
  - **Classification Report** (Precision, Recall, F1-score)

### 7️⃣ Feature Importance
- Ranked the most important features that influenced employment suitability.

---

## 📊 Results Summary

| Metric | Example Output |
|---------|----------------|
| **Accuracy** | 0.87 |
| **Top Features** | Interview Score, Technical Test Score, Years of Experience |

*Note: Actual metrics may vary based on dataset.*

---

## 🧠 Libraries Used
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`

---

## 🚀 How to Run

### 1️⃣ Install Dependencies
```bash
pip install pandas numpy matplotlib seaborn scikit-learn

