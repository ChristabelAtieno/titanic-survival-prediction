# Titanic Survival Prediction 🚢

This project uses machine learning to predict the survival of passengers on the Titanic based on features such as age, sex, class, and more.
The dataset comes from the [Kaggle Titanic competition](https://www.kaggle.com/competitions/titanic/data).

---
##  Datasets

- **train.csv**: Contains passenger details with the target column `Survived` (0 = did not survive, 1 = survived).  
- **test.csv**: Contains passenger details without the survival outcome (your task is to predict survival).  
- **gender_submission.csv**: A sample submission file provided by Kaggle for format reference.  

Key features include:
- **PassengerId**: Unique ID for each passenger  
- **Pclass**: Passenger class (1 = First, 2 = Second, 3 = Third)  
- **Name**: Passenger name  
- **Sex**: Gender of the passenger  
- **Age**: Age in years  
- **SibSp**: Number of siblings/spouses aboard  
- **Parch**: Number of parents/children aboard  
- **Ticket**: Ticket number  
- **Fare**: Ticket price  
- **Cabin**: Cabin number  
- **Embarked**: Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton)  

---

##  Steps Performed

1. **Data Loading** – Imported the datasets from the `datasets/` folder.  
2. **Data Preprocessing**  
   - Handled missing values (`Age`, `Cabin`, `Embarked`).  
   - Converted categorical features (`Sex`, `Embarked`) into numerical form.  
   - Dropped irrelevant features (`PassengerId`, `Name`, `Ticket`, `Cabin`).  
3. **Feature Engineering** – Created new features and scaled numerical data.  
4. **Modeling** – Trained multiple models to predict survival.  
5. **Evaluation** – Compared performance using accuracy scores.  
6. **Prediction** – Generated predictions for the `test.csv` dataset.  

---

##  Best Models

The following models were tested:
- Logistic Regression  
- Random Forest Classifier  
- Support Vector Machine (SVM)  
- GBoost  

✅ **Best performing model:**  
- **Random Forest Classifier** achieved the highest accuracy.  

---

##  Results & Insights

- **Gender was the most important factor**: Females had a much higher chance of survival.  
- **Passenger class (Pclass)** strongly influenced survival: First-class passengers survived more often.  
- **Younger passengers** had higher survival rates compared to older ones.  
- Random Forest provided the best performance, balancing interpretability and accuracy.  

---






