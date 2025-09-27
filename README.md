# 📌 Anomaly Detection in Financial Transactions  

## 🔎 Overview  
This project applies **unsupervised machine learning** to detect unusual customer behaviors in financial transaction data. While the dataset does not contain explicit fraud labels, anomalies can highlight **potentially risky or suspicious cases** that may require further investigation by financial institutions.  

---

## 🛠️ Tech Stack  
- **Python**: Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn  
- **Machine Learning**: Isolation Forest (anomaly detection), PCA (dimensionality reduction)  
- **Preprocessing**: Label Encoding, StandardScaler  

---

## 📊 Project Workflow  
1. **Data Cleaning & Preprocessing**  
   - Parsed dataset correctly (17 features, ~45,000 rows)  
   - Converted numeric columns, encoded categorical features, scaled features  

2. **Anomaly Detection**  
   - Applied **Isolation Forest** (`contamination=0.02`)  
   - Flagged ~2% of records as anomalies  

3. **Visualization & Reporting**  
   - **PCA scatterplot**: visual separation of anomalies vs normal cases  
   - **Pie chart**: anomaly vs normal distribution  
   - **Bar plots**: anomaly counts by job and education  
   - **Descriptive stats**: compared balance and age distributions  

---

## 📌 Results & Insights  
- **~2% anomalies detected** across the dataset  
- Anomalous customers often have:  
  - **Higher account balances**  
  - Slightly **older ages**  
  - Higher representation in **management & technician roles**  
- ⚠️ **Note**: Anomalies ≠ confirmed fraud. They indicate unusual behavior that could be investigated further.  

---

## ✅ Takeaways  
- Demonstrates how **unsupervised anomaly detection** can be applied in financial contexts  
- Provides a **risk prioritization framework** for analysts to narrow down suspicious cases  
- Clarifies the difference between **anomaly detection** (statistical outliers) and **fraud detection** (requires labeled fraud data)  

---

## 📂 Files  
- `bank-full.csv` → dataset (Bank Marketing data)  
- `bank_with_anomalies.csv` → processed dataset with anomaly flags  
- `bank_anomalies_only.csv` → extracted anomalies for further review  
- `notebook.ipynb` → full code and analysis  

---

## 🚀 Next Steps  
- Compare with other anomaly detection algorithms (One-Class SVM, Autoencoders)  
- Incorporate **transaction-level data** with explicit fraud labels  
- Evaluate model precision/recall once fraud labels are available  

---

✍️ **Author**: *Swastika P. K.*  
