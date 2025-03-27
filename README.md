# 🚀 Cybersecurity Threat Classification Using Machine Learning

## 📌 Project Overview
This project aims to detect **cybersecurity threats** using **Machine Learning** techniques. We have implemented **Random Forest** and **Support Vector Machine (SVM)** classifiers on network traffic data to classify attack and normal traffic.  

## 📂 Dataset Information
- The dataset contains **network traffic features** labeled as **attack** (1) or **normal** (0).
- **Preprocessing Steps:**
  - Removed unnecessary columns: `id`, `timestamp`, `src_ip`, `dst_ip`.
  - Standardized data for better model performance.

## 🛠️ Feature Selection
- **Correlation Analysis**: Identified and removed redundant features.
- **Random Forest Feature Importance**: Selected the most significant features.
- **Recursive Feature Elimination (RFE)**: Picked the top 5 best features.

## 🧠 Machine Learning Models
We trained and compared the following models:
- **Random Forest Classifier** (with GridSearchCV optimization)
- **Support Vector Machine (SVM)**

## 📊 Evaluation Metrics
| Model | Accuracy | Precision | Recall | F1-Score |
|--------|---------|-----------|--------|----------|
| Random Forest | 91% | 0.91 | 1.00 | 0.95 |
| SVM | 91% | 0.91 | 1.00 | 0.95 |

- **Confusion Matrices** showed that both models had trouble detecting attack cases due to class imbalance.

## 📈 Visualizations
- **Feature Correlation Matrix**
- **Feature Importance (Random Forest)**
- **Confusion Matrices for RF & SVM**

## ⚡ How to Run the Project
### **1️⃣ Install Dependencies**
```bash
pip install pandas numpy scikit-learn matplotlib seaborn
