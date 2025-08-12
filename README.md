## Customer Churn Prediction
 -   This project uses a Random Forest Classifier to predict whether a customer is likely to leave a business (churn) based on historical behavioral and demographic data.

**Goal:** Enable businesses to proactively identify at-risk customers and take retention measures.

Key Features:

Data preprocessing and feature engineering for improved model performance

Training and evaluation of a Random Forest Classifier

Visualization of feature importance for interpretability

Performance: Achieved 76% accuracy on the test dataset.

---

## 📂 Project Structure
data/ # Dataset files
notebooks/ # Jupyter notebooks with the full ML pipeline
models/ # Saved trained models and encoders
reports/ # Power BI dashboards


---

## 📊 Dataset
- **Name:** Telco Customer Churn
- **Features:** Customer demographics, service usage, and account details
- **Target:** `Churn` (Yes/No)
- **Size:** 7043 records × 21 columns

---

## 🛠 Methodology
1. **Data Loading** – Load CSV dataset using Pandas.
2. **EDA** – Visualize churn distribution and feature relationships with Seaborn/Matplotlib.
3. **Preprocessing**:
   - Encode categorical variables using `LabelEncoder`.
   - Handle class imbalance with **SMOTE**.
4. **Model Training**:
   - Models used: Decision Tree, Random Forest, XGBoost.
   - Hyperparameter tuning with `GridSearchCV`.
   - Cross-validation using `StratifiedKFold`.
5. **Evaluation**:
   - Accuracy, F1-score.
   - Confusion matrix.
   - Classification report.
6. **Model Saving**:
   - Save trained model as `customer_churn_model.pkl`.
   - Save encoders as `encoders.pkl`.

---

## 📊 Results
- **Best Model:** Random Forest  
- **Accuracy:** 76%  
- **F1-score (Churn class):** 0.72  
- **F1-score (Non-Churn class):** 0.78  
- Random Forest provided the most balanced performance across both classes after hyperparameter tuning.

---

## 🚀 How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/VedantKarande19/Customer_churn_prediction.git
   cd Customer_chur_prediction

2. Install dependencies:
   pip install -r requirements.txt


3. Open the Jupyter notebook:
   jupyter notebook notebook/Final_Customer_Churn_Prediction.ipynb

4. Run all cells to train and evaluate the model.
