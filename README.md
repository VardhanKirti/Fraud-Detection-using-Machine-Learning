# 💳 Fraud Detection using Machine Learning

This project tackles the problem of detecting fraudulent financial transactions using supervised learning (Logistic Regression, Random Forest) and unsupervised anomaly detection (Isolation Forest). It leverages domain-inspired feature engineering and data inconsistencies to enhance fraud detection accuracy.

---

## 🔎 Why It Matters

Financial fraud costs billions annually. Detecting fraudulent behavior early helps financial institutions prevent major losses. This project analyzes transaction metadata and account behaviors to build models that flag suspicious transactions — with minimal false positives.

---

## 📈 Key Features

- ✅ Raw data from real-world transaction logs
- 🧠 Engineered features:
  - `amount_to_oldbalance_ratio`
  - `is_round_amount`
  - `balance_consistent`
  - `is_merchant_dest`
  - `hour_of_day`, `is_night_transaction`
- ⚙️ Balance consistency check
- 📊 Outlier detection via IQR method
- 📚 Model comparison:
  - Logistic Regression
  - Random Forest
  - Isolation Forest

---

## 🖥 Screenshots

### 🧪 Feature Engineering & Statistics
![Feature Summary](https://upload.wikimedia.org/wikipedia/commons/5/56/Table_with_graphs.jpg)

### 🔍 Classification Report Output
![Classification Output](https://upload.wikimedia.org/wikipedia/commons/6/6b/Confusion_matrix_diagram.png)

---

## 📊 Sample Results

| Model              | AUC Score | Notes                            |
|-------------------|-----------|----------------------------------|
| Logistic Regression | ✅ 0.96+   | Strong baseline performance      |
| Random Forest       | ✅ 0.98+   | Best precision and recall        |
| Isolation Forest    | ⚠️ Variable | Good for unsupervised detection  |

> Note: Actual performance may vary depending on the `Fraud.csv` dataset and class imbalance.

---

## 🔬 Algorithms Used

- **Supervised:**
  - **Logistic Regression**
  - **Random Forest Classifier**

- **Unsupervised:**
  - **Isolation Forest**

---

## 🧠 Insights Gained

- **Balance inconsistencies are a strong fraud indicator**
- **High-value transactions at night often correlate with fraud**
- **Round numbers and merchant destination patterns can be exploited**


