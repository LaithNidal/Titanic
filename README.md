# 🚢 Titanic Survival Prediction (Kaggle + Streamlit App)

## 📘 Overview
This project predicts whether a passenger would have survived the Titanic disaster using machine learning.  
It includes:
- A **Jupyter Lab Notebook** for model development and analysis (`PSUT_Titanic_ML_Project.ipynb`)
- A **Streamlit web app** (`streamlit_app.py`) for interactive predictions

---

## 🧠 Objective
Build a supervised machine learning model to predict survival outcomes based on passenger demographics and trip information.Then make streamlit domain to host ML model on other users based  of their key features. 

**Goal:** Classify survival (1 = Survived, 0 = Did not survive)

---

## 🧩 Datasets
Source: [Kaggle Titanic Dataset](https://www.kaggle.com/competitions/titanic/data)

**Files Used:**
- `train_cleaned.csv` – Training data
- `test_cleaned.csv` – Test data

Key features:
- `Pclass`: Passenger class (1, 2, 3)
- `Sex`: Gender (0 = male, 1 = female)
- `Age`: Passenger age
- `SibSp`: Number of siblings/spouses aboard
- `Parch`: Number of parents/children aboard
- `Fare`: Ticket price
- `Embarked`: Port of Embarkation (0 = Southampton, 1 = Cherbourg, 2 = Queenstown)

---

## ⚙️ Model Pipeline

1. **Data Cleaning & Preprocessing**
   - Missing values handled
   - Feature encoding
   - Standardization using `StandardScaler`

2. **Model Training**
   - Split dataset into training and validation sets (80/20)
   - Two models tested:
     - **Logistic Regression**
     - **Random Forest Classifier**

3. **Model Evaluation**
   - Accuracy measured on validation set
   - Random Forest generally performed best in tests

---

## 🧾 Notebook Summary (`PSUT_Titanic_ML_Project.ipynb`)
- Exploratory Data Analysis (EDA)
- Feature engineering and correlation visualization
- Model selection and testing.
- Both models gave an **accuracy of 82.4%.** 

---

## 🌐 Streamlit Web App (`streamlit_app.py`)
### Features:
- Interactive user input for passenger details
- Real-time prediction output
- Side panel to select ML model and adjust parameters

### How It Works:
1. User enters passenger info:
   - Class, Gender, Age, Family Members, Fare, Embarkation
2. Selects model type (Logistic Regression or Random Forest)
3. Clicks **Predict**
4. App displays survival prediction (0 = Death, 1 = Survival)
