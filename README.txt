# 💳 Credit Card Fraud Detection using Machine Learning

> A machine learning project to detect fraudulent credit card transactions using **Logistic Regression** and **SMOTE** — effectively handling extreme class imbalance and improving fraud recall.

---

## 📁 Project Overview

Credit card fraud is a critical challenge in the financial sector. Fraudulent transactions account for less than **0.2%** of the total, making this a **highly imbalanced classification** problem.

This project uses a real-world anonymized dataset and applies:
- Exploratory Data Analysis (EDA)
- Feature Scaling
- Logistic Regression
- SMOTE (Synthetic Minority Oversampling)
- Evaluation using Precision, Recall, F1-score

---

## 📊 Dataset

- Source: [https://skillfiedmentor.com/portal]
- 284,807 transactions
- 30 features (`V1` to `V28`, `Time`, `Amount`)
- Target: `Class` → `1 = Fraud`, `0 = Non-Fraud`

---

## ⚙️ Project Workflow

```plaintext
1. Load Data
2. EDA: Distribution & Correlation
3. Preprocessing:
   - Feature scaling (Time, Amount)
4. Train-Test Split (Stratified)
5. Model 1: Logistic Regression (raw data)
6. Handle Imbalance: Apply SMOTE
7. Model 2: Logistic Regression (SMOTE data)
8. Evaluation: Compare metrics before vs after SMOTE
```

---

## 📈 Results

| Metric    | Before SMOTE | After SMOTE |
| --------- | ------------ | ----------- |
| Accuracy  | 0.96         | 0.60        |
| Recall    | 0.61         | 0.84 ✅      |
| Precision | High         | Moderate    |
| F1-Score  | Low          | Improved ✅  |

> SMOTE significantly improves recall, which is crucial for catching fraud cases.

---

## 🛠️ Tech Stack

* **Language**: Python 3.x
* **Libraries**:

  * `pandas`, `numpy`
  * `matplotlib`, `seaborn`
  * `scikit-learn`
  * `imblearn` (SMOTE)

---

## 📁 File Structure

```bash
.
├── Credit_Card_Fraud_Detection.ipynb   # Main notebook
├── README.md                           # This file
├── images/                             # Visuals used in project
│   ├── correlation_heatmap.png
│   ├── class_distribution.png
│   └── smote_results.png
```

---

## 📌 Key Learnings

* How to handle **imbalanced datasets**
* Importance of **recall** in fraud detection
* Using **SMOTE** to improve minority class performance
* How to interpret model evaluation metrics effectively

---

## 👩‍💻 Author

**Namrata Dolas**  
*Data Science Intern*  
B.Tech in Electronics Engineering
🔗 [GitHub](https://github.com/Namrata-Dolas19/Credit-Card-Fraud-Detection)

---

## ⭐️ If you liked this project, consider giving it a star!

Let me know your feedback or suggestions — always open to collaboration!
