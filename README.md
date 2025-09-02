# titanic-machine-learning

This project applies **Machine Learning** techniques to the famous **Titanic dataset** to predict whether a passenger survived or not.  

## 📌 Project Structure  
- **titanic predicit.ipynb** → Main notebook with preprocessing, feature engineering, modeling, and evaluation.  
- **README.md** → Project description and documentation.  
- **requirements.txt** → Python dependencies (to be added).  

## 🧹 Data Preprocessing  
- Dropped irrelevant features: `PassengerId`, `Name`, `Cabin`, `Ticket`.  
- Filled missing values:  
  - `Age` → Median value.  
  - `Embarked` → Mode value.  
- Encoded categorical features:  
  - `Sex` → Label Encoding.  
  - `Embarked` → One-Hot Encoding.  
- Engineered new feature: `FamilySize = SibSp + Parch`.  
- Handled outliers with **IQR method**.  
- Scaled features before applying some models.  

## 🤖 Models Applied  
- Logistic Regression  
- KNN  
- Decision Tree / Extra Trees  
- Random Forest  
- Gradient Boosting  
- XGBoost  
- LightGBM  
- Support Vector Machine (SVM)  

## 🏆 Best Model  
- **Support Vector Machine (SVM)** achieved the highest accuracy.  
- **Accuracy:** ~87%  
- **Precision/Recall/F1:**  
  - Class 0 (Not Survived): Precision = 0.85, Recall = 0.93  
  - Class 1 (Survived): Precision = 0.87, Recall = 0.75  

## 📊 Evaluation  
- Classification report (accuracy, precision, recall, F1-score).  
- Confusion matrix visualization for better interpretability.  
