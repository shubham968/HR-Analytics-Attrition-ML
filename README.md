# HR-Analytics-Attrition-ML# HR Attrition Prediction 🔍💼

This project is a Machine Learning pipeline built to predict **employee attrition** using an HR dataset from [Kaggle](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset). The goal is to identify patterns and risk factors that lead to employee churn, helping organizations take proactive steps for retention.

---

## 📁 Dataset

- **Source**: IBM HR Analytics Employee Attrition & Performance (Kaggle)
- **Records**: ~1,470 employees
- **Target Variable**: `Attrition` (Yes/No)

---

## 🔧 Workflow

1. **Data Loading & Exploration**
   - Checked for nulls, data types, and initial patterns using `pandas` and `matplotlib/seaborn`.
   
2. **Preprocessing**
   - Encoded categorical features using `OneHotEncoder`.
   - Scaled numerical features using `StandardScaler`.
   - Label encoded the target column (`Attrition`) for classification.

3. **Train-Test Split**
   - Used `train_test_split` with 70/30 split.

4. **Model Building**
   - Applied multiple models:
     - Logistic Regression
     - XGBoost Classifier ✅ (Best Accuracy: ~99%)

5. **Evaluation**
   - Metrics used:
     - Accuracy Score
     - Confusion Matrix
     - Classification Report

6. **Feature Importance**
   - XGBoost feature importance plot helped interpret key drivers of attrition.

---

## 📊 Results

- **Best Model**: XGBoost Classifier
- **Accuracy**: ~99%
- **Top Features**:
  - OverTime
  - JobRole
  - YearsSinceLastPromotion
  - Age

---

## 📦 Tech Stack

- Python
- Pandas, NumPy
- Scikit-learn
- XGBoost
- Matplotlib, Seaborn
- Jupyter Notebook

---

## 💡 Future Improvements

- Hyperparameter tuning
- SHAP or LIME for deeper interpretability
- Integration with a Streamlit dashboard
- Fetching real-time data from SQL or API sources



---

## 🤝 Contributions

If you have ideas for improving this project, feel free to fork the repo, open issues, or submit a pull request!

---

## 📜 License

This project is open-source and available under the MIT License.
