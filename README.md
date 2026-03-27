# Healthcare-Data-Preprocessing-Feature-Engineering
Cleaning and feature engineering on synthetic healthcare data to handle PII and prepare for ML.
## 🎯 Project Objective
This project demonstrates a complete end-to-end workflow for cleaning and preparing messy, real-world healthcare data for machine learning. The primary focus is on maintaining data quality while ensuring patient privacy (PII removal) and compliance with standards like HIPAA and GDPR.

## 📂 Project Structure
The project is divided into two main stages:

### 1. Simple Overview (`1_Simple_Overview.ipynb`)
A beginner-friendly introduction to the dataset.
* **Initial Exploration:** Loading the 200-record synthetic dataset.
* **Basic Cleaning:** Identifying common issues like missing values and inconsistent categorical labels (e.g., standardizing "M", "f", "Male" to a single format).

### 2. Advanced Preprocessing & Engineering (`2_Deep_Feature_Engineering.ipynb`)
A deep dive into preparing data for production-level Machine Learning.
* **Privacy First (PII Removal):** Removing sensitive columns like `Patient_Name` and `EmailID`.
* **Handling Data Quality:** Systematic removal of duplicates and handling outliers (e.g., Age = 200).
* **Feature Engineering:** Creating domain-specific features like **BMI** from height and weight and extracting time-based features from diagnosis dates.
* **ML Preparation:** Applying `StandardScaler` for numerical scaling and `OneHotEncoder` for categorical variables.

## 🛠️ Tech Stack
* **Language:** Python
* **Libraries:** Pandas, NumPy, Scikit-Learn, SciPy.

## 📊 The Dataset
The dataset is intentionally designed to be "messy" to simulate real Electronic Health Record (EHR) systems. It includes:
* **Missing values** (Age, Weight).
* **Mixed units** (kg vs lbs).
* **Typos** (e.g., "ANX" vs "ANXITY").
* **Multiple date formats**.

## ✅ Final Result
The project transforms raw, unsafe medical data into a clean, consistent, and privacy-compliant dataset ready for predictive modeling (e.g., disease risk prediction).
