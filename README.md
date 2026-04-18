# 🌧️ Rainfall Prediction for Agriculture (DS Project)

## 📌 Project Overview

This project applies **data science and machine learning techniques** to analyze historical rainfall data in India (1901–2015) and build predictive models to support agricultural and urban planning decisions.

Using the **CRISP-DM methodology**, the project explores long-term rainfall patterns, detects extreme weather events, and builds models to predict rainfall anomalies such as droughts and heavy rainfall conditions.

---

## 🎯 Business Objectives

### Q1: Crop Planning (Prediction Task)

Predict whether a region will experience:

- 🌵 Drought conditions (below-normal rainfall)
- 🌧️ Heavy rainfall conditions (above-normal rainfall)

📌 Goal: Support farmers in crop selection, irrigation planning, and risk reduction.

---

### Q2: Urban Planning (Research Task)

Analyze whether extreme rainfall events have increased over the past 30 years.

📌 Goal: Support flood risk management and infrastructure planning.

---

## 📊 Dataset

- **Source:** Rainfall in India (1901–2015)
- **Type:** Time-series / regional rainfall data
- **Features:** Monthly and annual rainfall statistics across Indian regions

---

## 🧠 Machine Learning Approach

### Problem Type:

- Q1 → Classification (Drought / Normal / Heavy Rainfall)
- Q2 → Time-Series Trend Analysis

### Models Used:

- Linear Regression (baseline)
- Random Forest
- Gradient Boosting
- (Optional) Hyperparameter tuning with GridSearchCV

---

## 🏗️ Project Structure

Rainfall-Prediction-for-Agriculture-DS/
│
├── data/
│ ├── raw/
│ └── processed/
│
├── notebooks/
│ ├── 01_Business_Understanding.ipynb
│ ├── 02_Data_Understanding.ipynb
│ ├── 03_Data_Preparation.ipynb
│ ├── 04_Modelling.ipynb
│ ├── 05_Evaluation.ipynb
│ └── 06_Deployment.ipynb
│
├── src/
│ ├── processing.py
│ ├── features.py
│ └── utils.py
│
├── models/
│ └── rainfall_model.pkl
│
├── README.md
└── requirements.txt

---

## 🔄 CRISP-DM Workflow

### 1. Business Understanding

Defined agricultural and climate-related objectives and success criteria.

### 2. Data Understanding

Explored rainfall trends, missing values, and extreme event patterns.

### 3. Data Preparation

- Data cleaning (missing values, inconsistencies)
- Feature engineering (rainfall deviation, anomaly labeling)
- Encoding and scaling

### 4. Modelling

- Train/test split
- Model training and comparison
- Hyperparameter tuning

### 5. Evaluation

- Model performance evaluated using:
  - Accuracy
  - Precision / Recall
  - F1-score
  - R² Score (for regression tasks)

### 6. Deployment

- Model saved using `joblib`
- Prediction pipeline created
- Deployment-ready inference function implemented

---

## 📈 Key Features

- Detection of rainfall anomalies (drought / heavy rainfall)
- Time-series analysis of extreme weather events
- Machine learning prediction pipeline
- CRISP-DM structured workflow
- Modular Python code design

---

## ⚙️ Technologies Used

- Python 🐍
- Pandas / NumPy
- Scikit-learn
- Matplotlib / Seaborn
- Jupyter Notebook
- Git & GitHub

---

## 🚀 How to Run the Project

### 1. Clone the repository

2. Install dependencies
   pip install -r requirements.txt
3. Run notebooks

Open Jupyter or VS Code and execute notebooks in order:

01 → 02 → 03 → 04 → 05 → 06
📌 Model Deployment

The trained model is saved using:

import joblib
joblib.dump(model, "models/rainfall_model.pkl")

To load the model:

model = joblib.load("models/rainfall_model.pkl")

⚠️ Limitations
Limited external climate features (temperature, ENSO, etc.)
Historical data may not fully reflect modern climate change dynamics
Class imbalance in extreme rainfall events

🔮 Future Improvements
Integrate weather APIs for real-time prediction
Add deep learning models (LSTM for time-series)
Improve geospatial analysis using GIS tools
Deploy as a web application (Flask/FastAPI)

👨‍💻 Author

Mohamed Gdoura
