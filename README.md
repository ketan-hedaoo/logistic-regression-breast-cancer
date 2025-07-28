# 🩺 Breast Cancer Detection using Logistic Regression

## 📌 Project Overview
This project uses **Logistic Regression** to classify breast tumors as **malignant (1)** or **benign (0)** using features from the **Breast Cancer Wisconsin dataset** (`sklearn.datasets.load_breast_cancer`).

In medical problems, **recall (sensitivity)** is crucial to minimize **false negatives** (i.e., missing malignant tumors).  
We also analyze different probability thresholds to optimize classification.

---

## 📂 Dataset
- **Source:** `sklearn.datasets.load_breast_cancer()`
- **Features:** 30 numerical features describing cell nuclei characteristics.
- **Target:**  
  - `1` → Malignant (disease present)  
  - `0` → Benign (no disease)

---

## 🔄 Workflow
1. **🔍 Exploratory Data Analysis (EDA)**
   - Class distribution visualization.
   - Correlation analysis for top features.
   - Boxplots for important features.

2. **⚙️ Data Preprocessing**
   - Train-test split (80-20 stratified).
   - Feature scaling using **StandardScaler**.

3. **🤖 Model Building**
   - Logistic Regression (solver = `liblinear`, random_state = 42).
   - Model saved using `joblib`.

4. **📊 Model Evaluation**
   - Default threshold (0.5) → Confusion matrix, classification report, ROC-AUC.
   - Best threshold (max accuracy) search.
   - Critical threshold → Ensures **no false negatives** (100% recall).

---

## 🛠 Tech Stack
- **Programming Language:** Python 3
- **Libraries:**  
  - pandas, numpy  
  - matplotlib, seaborn  
  - scikit-learn  
  - joblib

