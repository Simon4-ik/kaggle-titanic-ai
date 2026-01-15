# 🚢 Kaggle Titanic – Machine Learning from Disaster

## 👤 Username
mnozimjo01EDU_astana_01_2026
(Stored in `username.txt`, unchanged after day 1)

## 📌 Project Overview
This project is part of a 1-week Data Science challenge based on the Kaggle competition  
**“Titanic: Machine Learning from Disaster”**.

The goal is to build a machine learning model that predicts which passengers survived the Titanic shipwreck using passenger data such as age, gender, class, and family relations.

## 🎯 Objective
- Perform data analysis and feature engineering
- Train and evaluate machine learning models
- Submit predictions to Kaggle
- Achieve **at least 78.9% accuracy** on the Kaggle leaderboard

## 📊 Best Kaggle Score
- **Leaderboard accuracy:** `77.5%`
- **Validation accuracy (cross-validation):** `78.9%`
- Same pipeline was used for both validation and Kaggle submission

## 🧠 Feature Engineering
Key features used in the final model:
- **Sex** (encoded)
- **Pclass**
- **Age** (filled using median values)
- **FamilySize** = SibSp + Parch + 1
- **IsAlone** (derived from FamilySize)
- **Fare** (log-transformed)
- **Embarked** (filled with most frequent value)
- **Title** extracted from passenger names (Mr, Mrs, Miss, etc.)

These features were chosen to reflect social status, survival priority, and family context during the disaster.

## 🤖 Model
- Algorithm used: **Logistic Regression / Random Forest / XGBoost**  
- Hyperparameters tuned using cross-validation
- Overfitting checked by splitting training data

## 📁 Project Structure
project
│   README.md
│   requirements.txt
│   username.txt
│
└───data
│   │   train.csv
│   |   test.csv
|   |   gender_submission.csv
│
└───notebook
│   │   main.ipynb


## 📓 Notebook (`main.ipynb`)
The notebook contains:
- Data loading and exploration
- Feature engineering experiments
- Model training and evaluation
- Cross-validation
- Final prediction on test data
- Kaggle submission file generation

All steps are clearly commented and reproducible.

## ⚙️ Installation & Run
```bash
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
jupyter notebook
Then open:

notebook/main.ipynb