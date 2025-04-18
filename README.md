# Predict-Employee-Attrition
# 🧠 Employee Attrition Prediction

Predict employee attrition using machine learning to help HR departments take proactive action in retaining key talent.

---

## 📌 Project Title
**Predicting Employee Attrition Using Machine Learning**

---

## 🧠 Objective

This project aims to build a machine learning classification model that predicts whether an employee is likely to leave a company. The model uses features such as job satisfaction, salary, work environment, and years of experience. The goal is to assist HR teams in reducing employee turnover through data-driven decisions.

---

## 📂 Dataset Description

The dataset (`6. Predict Employee Attrition.csv`) contains the following key features:

- `JobSatisfaction` – Rating of employee job satisfaction  
- `Salary` – Employee annual salary  
- `WorkEnvironment` – Quality of the work environment (scored)  
- `YearsExperience` – Total work experience of the employee  
- `Attrition` – Target variable (Yes = employee left, No = stayed)  

---

## 🧹 Data Preprocessing

- **Missing Values**: Rows with missing values were removed  
- **Target Encoding**: Converted `Attrition` from Yes/No to 1/0  
- **Categorical Encoding**: Used one-hot encoding with `pd.get_dummies()`  
- **Feature Scaling**: Standardized features using `StandardScaler`  

---

## ⚙️ Model Building

- **Model**: Logistic Regression  
- **Train/Test Split**: 80% training, 20% testing  
- **Hyperparameters**: `max_iter=1000` to ensure convergence  

---

## 📊 Visualizations

- **Attrition Distribution**: Visualizes balance between stayed vs left  
- **Correlation Heatmap**: Displays feature correlations  
- **Feature Importance**: Shows coefficients from logistic regression  
- **Confusion Matrix**: Visualizes prediction performance  

---

## 📈 Model Evaluation

| Metric     | Score              |
|------------|--------------------|
| Accuracy   | ~85–90%*           |
| Precision  | Based on test set  |
| Recall     | Based on test set  |
| AUC-ROC    | Optional extension |
| Confusion Matrix | Visualized using seaborn |

> \* Accuracy may vary based on dataset composition.

---

## ✅ Key Insights

- Job satisfaction and years of experience are highly predictive of attrition.
- Logistic regression provides a transparent, interpretable model.
- Strong baseline results can be improved with more advanced models.

---

## 💡 Future Enhancements

- Try models like **Random Forest**, **XGBoost**, or **Neural Networks**
- Use **SMOTE** or other techniques to handle class imbalance
- Deploy a **web interface** for real-time HR insights
- Add **explainability** with SHAP or LIME

---

## 🧾 Conclusion

This project demonstrates a reliable method to predict employee attrition using historical data. By identifying potential leavers, organizations can intervene early and optimize retention strategies.

---

## 📁 Project Structure

```bash
├── data/
│   └── 6. Predict Employee Attrition.csv
├── notebooks/
│   └── EDA_and_Model.ipynb
├── src/
│   └── preprocessing.py
│   └── model.py
├── visuals/
│   └── feature_importance.png
│   └── confusion_matrix.png
├── README.md
└── requirements.txt
