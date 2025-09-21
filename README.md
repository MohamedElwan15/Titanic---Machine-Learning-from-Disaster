# 🛳️ Titanic - Machine Learning from Disaster
####  Predicting Titanic Survivors with Machine Learning

## 📌 Overview
This project tackles the famous Kaggle Titanic competition, where the goal is to predict whether a passenger survived the Titanic shipwreck using passenger data (age, sex, class, etc.).

It showcases key steps in a typical machine learning workflow: data cleaning, feature engineering, model selection, and evaluation.

## 🗂️ Dataset

train.csv – Passenger data with survival labels (used for training & validation).

test.csv – Passenger data without labels (used for Kaggle submission).

Provided by Kaggle.

## 🔧 Key Steps

### Data Cleaning

Handled missing values (Age, Embarked, Fare) with appropriate imputations.
Dropped irrelevant columns (e.g., Cabin, Ticket).

### Feature Engineering
Extracted Title from names (Mr, Mrs, Miss, Master, Rare).
Created Family_Size (SibSp + Parch + 1).
Created Is_Alone (1 if Family_Size = 1, else 0).
Converted categorical variables to numeric using one-hot encoding.

## Modeling
Logistic Regression as the baseline model.
Tuned hyperparameter C using GridSearchCV for better regularization.

## Evaluation

Scored 0.78229 on Kaggle’s public leaderboard (Top ~20% on second submission 🎯).

## 📈 Results
| Submission | Score (Accuracy) | Rank (out of 13,000+)  |
| ---------- | ---------------- | ------ |
| First try  | **0.76794**      | \~8947 |
| Second try | **0.78229**      | \~2347 |

### 💡 Next Improvements
Explore advanced models (Random Forest, XGBoost).
Feature interactions & more sophisticated feature scaling.
Ensemble methods for higher accuracy.

## 🏆 Leaderboard
My second submission reached a score of 0.78229 with Logistic Regression + feature engineering.

### 🚀 How to Run
Clone the repo

git clone https://github.com/MohamedElwan15/Titanic---Machine-Learning-from-Disaster
cd titanic-ml

Run the notebook to reproduce results.

## 🙋‍♂️ Author

Mohamed Elwan – [Kaggle Profile](https://www.kaggle.com/mohamedelwan15)
 | [LinkedIn](https://www.linkedin.com/in/m-elwan/)
