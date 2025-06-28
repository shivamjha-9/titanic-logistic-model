# 🛳 Titanic Survival Prediction | Logistic Regression with Scikit‑learn

Predicting passenger survival on the Titanic using logistic regression. This project covers data cleaning, feature engineering, model training, evaluation, and result interpretation using Python and Scikit‑learn.

---

## 📊 Dataset
- **Source**: Kaggle *“Titanic – Machine Learning from Disaster”*
- **Train Data**: 891 passengers with survival response
- **Test Data**: 418 passengers (without labels)
- **Key Features**: Pclass, Sex, Age, SibSp, Parch, Fare, Embarked

---

## 🔧 Technologies & Libraries
- Python 3
- Pandas, NumPy
- Scikit-learn
- Seaborn & Matplotlib

---

## 🧠 Approach & Pipeline
1. **Data Preprocessing**  
   - Dropped irrelevant columns (Cabin, Ticket, Name, etc.)  
   - Imputed missing values (mean Age, most common Embarked)  
   - Encoded categorical features (`Sex`, `Embarked`) using one-hot encoding  
   - Standardized numeric features (Age, Fare) using StandardScaler

2. **Model Building**  
   - Split into train/test sets (80/20)  
   - Trained `LogisticRegression` model  
   - Visualized model coefficients for feature importance

3. **Evaluation**  
   - Obtained training and test accuracy (~82.8% / ~76.2%)  
   - Generated classification report and confusion matrix  
   - Analyzed misclassification and feature impact

---

## 📈 Results

| Metric               | Value       |
|----------------------|-------------|
| Training Accuracy    | ~82.8%      |
| Test Accuracy        | ~76.2%      |

📌 **Insight**: Logistic regression effectively predicts survival based on Sex, Pclass, Age, and SibSp. Significant coefficients confirm historical survival trends.

---

## 📚 Key Learnings
- Handling missing data and categorical features  
- Importance of feature scaling for logistic regression  
- Model evaluation using classification metrics  
- Interpreting feature importance from model coefficients

---

## 🧩 File Structure

├── Titanic_Survived__Prediction.ipynb # Main Jupyter notebook
├── images/ # (Optional) EDA & evaluation plots
│ └── confusion_matrix.png
├── README.md # This documentation

---

## ⚙️ How to Run
1. Clone the repository  
   ```bash
   git clone https://github.com/shivamjha-9/titanic-logistic-model.git

