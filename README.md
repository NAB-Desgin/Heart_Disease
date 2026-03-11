# ❤️ Heart Disease Prediction – Exploratory Data Analysis & Preprocessing

A data analysis and preprocessing project that explores a heart disease dataset to understand the factors influencing heart disease and prepares the data for machine learning models.

This project focuses on:

Exploratory Data Analysis (EDA)

Data Cleaning

Feature Understanding

Statistical Analysis

Preparing the dataset for Machine Learning

# 📌 Project Overview

Heart disease is one of the leading causes of death worldwide. Understanding the key medical indicators can help predict and prevent heart-related conditions.

This project performs data exploration and preprocessing on a heart disease dataset to identify patterns and relationships between patient attributes and heart disease risk.

The notebook includes:

Dataset inspection

Handling missing or abnormal values

Exploratory visualizations

Statistical analysis

Feature preparation for ML models

# 📂 Dataset

The dataset used in this project contains medical attributes related to heart health.

Example Features
Feature	Description
Age	Age of the patient
Sex	Gender of the patient
ChestPainType	Type of chest pain experienced
RestingBP	Resting blood pressure
Cholesterol	Serum cholesterol level
FastingBS	Fasting blood sugar
RestingECG	Resting electrocardiogram results
MaxHR	Maximum heart rate achieved
ExerciseAngina	Exercise induced angina
Oldpeak	ST depression induced by exercise
ST_Slope	Slope of peak exercise ST segment
HeartDisease	Target variable (1 = Disease, 0 = No Disease)
🔍 Exploratory Data Analysis (EDA)

# EDA is performed to understand the structure, distribution, and patterns in the dataset.

Key Steps

Dataset overview

Checking shape and columns

Statistical summary

Detecting duplicates

Missing value analysis

Target variable distribution

Example analysis:

df.shape
df.info()
df.describe()
# 🧹 Data Cleaning

Data preprocessing is essential to ensure data quality before model training.

Steps performed

✔ Handling duplicate rows
✔ Checking missing values
✔ Replacing incorrect values

Example:

Some cholesterol values were 0, which is medically unrealistic.

These values were replaced using the mean cholesterol value:

ch_mean = df.loc[df['Cholesterol'] != 0, 'Cholesterol'].mean()
df['Cholesterol'] = df['Cholesterol'].replace(0, ch_mean)
# 📊 Data Visualization

Visualizations help understand patterns and relationships in the dataset.

Examples used in the project:

Target variable distribution

Feature value counts

Relationship between medical indicators and heart disease

Example visualization:

df['HeartDisease'].value_counts().plot(kind="bar")

This helps observe the balance between patients with and without heart disease.

# 🧠 Feature Analysis

Different features are analyzed to understand how they relate to heart disease.

Examples:

Sex distribution

Cholesterol levels

Blood pressure

Chest pain types

Heart rate patterns

Feature relationships help determine which variables may influence heart disease risk.

# ⚙️ Feature Preparation

The dataset is prepared for machine learning by:

Cleaning invalid values

Handling categorical features

Creating meaningful feature representations

Preparing structured data for modeling


# 🚀 How to Run the Project
1️⃣ Clone the repository
git clone https://github.com/NAB-Desgin/Heart_Disease.git
2️⃣ Navigate to the project folder
cd Heart_Disease
3️⃣ Install required libraries
pip install pandas numpy matplotlib seaborn scikit-learn
4️⃣ Run the notebook

Open:

heart_disease.ipynb

in Jupyter Notebook or VS Code.

🛠 Technologies Used

Python

Pandas

NumPy

Matplotlib

Seaborn

Jupyter Notebook

📈 Future Improvements

Future improvements to this project may include:

Machine Learning model training

Model comparison

Feature importance analysis

Hyperparameter tuning

Model evaluation metrics

Building a heart disease prediction system

# 📊 Potential Machine Learning Models

This dataset can be used to train models such as:

Logistic Regression

Random Forest

Decision Trees

Support Vector Machine

Gradient Boosting

# 🎯 Project Goals

The goal of this project is to:

Understand medical indicators of heart disease

Perform real-world dataset preprocessing

Prepare data for machine learning

Build a foundation for predictive healthcare models

# 👨‍💻 Author

NAB Design

GitHub Repository
https://github.com/NAB-Desgin/Heart_Disease
