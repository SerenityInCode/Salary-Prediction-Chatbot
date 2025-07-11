# 💼 Salary Prediction Chatbot (Freshers Edition)

A machine learning-based chatbot that predicts salaries for entry-level positions (0–1 year of experience) using job title, country, and education level. Built with Python and trained on real-world salary data, this project offers salary insights in an interactive, conversational format.

---

## 📌 Project Overview

This chatbot accepts key user inputs:
- **Job Title**
- **Country**
- **Education Level**

It processes this information and uses a trained **Random Forest Regressor** to estimate an appropriate salary for freshers. The chatbot is designed for individuals just entering the workforce, including recent graduates and early-career professionals.

---

## 📊 Dataset

- **Source**: [Kaggle Salary Dataset (Salary by Job Title and Country)](https://www.kaggle.com/datasets/amirmahdiabbootalebi/salary-by-job-title-and-country)
- **Key Columns Used**:
  - `Job Title`
  - `Country`
  - `Education Level`
  - `Salary`
- **Preprocessing**:
  - Dropped irrelevant columns: `Race`, `Senior`
  - Filtered for freshers (`Years of Experience` = 0 or 1)
  - Converted salary and experience data to `int64`

---

## 🔍 Workflow Summary

1. **Load and Clean Data**
2. **Filter for Freshers (0–1 year experience)**
3. **Encode Categorical Features using OneHotEncoder**
4. **Train a Random Forest Regressor**
5. **Build Chatbot Interface to Collect User Inputs**
6. **Predict and Display Estimated Salary**

---

## 🧠 Model Details

- **Model**: `RandomForestRegressor` from scikit-learn
- **Encoder**: `OneHotEncoder` via `ColumnTransformer`
- **Pipeline**: Preprocessing + Model
- **Target Variable**: `Salary`

---

## 💬 Example Interaction

<img width="942" height="617" alt="image" src="https://github.com/user-attachments/assets/a327a172-a5ec-42f1-afc5-057ff4705cc5" />
