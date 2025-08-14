# Breast Cancer Survival Prediction – Machine Learning Project

## 📌 Project Overview
This project applies **Machine Learning and Data Mining** techniques to predict:
1. **Mortality Status** (Alive/Dead) – *Classification*
2. **Survival Months** – *Regression*

The work is based on a healthcare dataset containing demographic, clinical, and pathological information of breast cancer patients. The models aim to support **clinical decision-making** and **early prognosis**, especially in low-resource healthcare settings.

---

## 🎯 Objectives
- Build classification models to predict mortality status using clinical data.
- Build regression models to estimate survival months after diagnosis.
- Compare and evaluate multiple ML algorithms.
- Provide interpretable outputs for healthcare professionals.

---

## 📂 Case Studies

### **Case Study A – Classification**
**Goal:** Predict whether a patient is Alive or Dead.

#### Steps:
1. **Domain Understanding** – Identify relevant features for classification.
2. **Data Preparation** – Handle missing values, encode categorical variables, and scale data.
3. **Modeling** – Algorithms used:
   - Gaussian Naive Bayes (NB)
   - Logistic Regression (LR)
   - K-Nearest Neighbors (KNN)
4. **Evaluation** – Used metrics:
   - Recall, Precision, F1-Score, AUC-ROC
5. **Best Model:** Logistic Regression (AUC-ROC: 0.739, Recall: 0.99)

---

### **Case Study B – Regression**
**Goal:** Predict the number of months a patient survives after diagnosis.

#### Steps:
1. **Domain Understanding** – Survival months as a continuous variable.
2. **Modeling** – Decision Tree Regression with pre-pruning (`max_depth=5`).
3. **Evaluation** – Used metrics:
   - Mean Squared Error (MSE)
   - Mean Absolute Error (MAE)
   - R² Score
4. **Best Model:** Decision Tree Regressor (R² = 0.68)

---

## 📊 Dataset Preparation
- Removed irrelevant identifiers (e.g., Patient ID, Month of Birth)
- Imputed missing values with median
- Encoded categorical variables
- Standardized numerical features
- Stratified 80:20 train-test split with `random_state=42`

---

## 🛠️ Technologies Used
- **Python** (Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn)
- **Jupyter Notebook**
- **Decision Tree Visualization** (`plot_tree`)
- **Data Preprocessing** (Label Encoding, StandardScaler)
- **ML Models**: Naive Bayes, Logistic Regression, KNN, Decision Tree Regressor

---

## 📈 Key Results
- **Classification:** Logistic Regression provided balanced, interpretable, and reliable predictions.
- **Regression:** Decision Tree Regressor offered interpretable predictions for survival months.
- **Ethical Considerations:** Model use in healthcare must ensure fairness, interpretability, and patient well-being.

---

## 📌 Limitations
- Limited feature set – may not capture all clinical variables.
- Dataset representativeness – possible demographic biases.
- Ethical risks in communicating mortality predictions.
- Potential overfitting in tuned KNN model.

---

## 📜 References
- [The Lancet – Tamoxifen Efficacy Study](https://doi.org/10.1016/S0140-6736(11)60993-8)
- AJCC Cancer Staging Manual, 7th Edition
- Breast Cancer Research Journal
- CA: A Cancer Journal for Clinicians

---

## 🚀 How to Run
1. Clone this repository:
   ```bash
   git clone <repo-url>
   cd <repo-folder>
