# Cyber_Threat_Classification_Using_Machine_Learning

 Cybersecurity Threat Classification Using Machine Learning
📌 Project Overview
This project focuses on cybersecurity threat classification using machine learning. The goal is to detect cyber-attacks based on network traffic data using Random Forest and Support Vector Machines (SVM).

📂 Dataset
The dataset contains network traffic features labeled as attack or normal.

Features like src_ip, dst_ip, and timestamp were removed as they were not relevant for classification.

🛠️ Preprocessing & Feature Selection
Data Cleaning: Removed unnecessary columns (id, timestamp, src_ip, dst_ip).

Feature Selection:
Correlation Analysis: Identified redundant features.
Random Forest Feature Importance: Selected key features.
Recursive Feature Elimination (RFE): Picked the top 5 important features.

🧠 Machine Learning Models Used
Random Forest Classifier (Baseline & Optimized with GridSearchCV)
Support Vector Machine (SVM)

📊 Evaluation & Results
  Model       	Accuracy  	Precision 	Recall	 F1-Score
Random Forest	: 91%	       0.91	       1.00	      0.95
SVM:            91%	       0.91       	1.00	      0.95
Confusion matrices showed poor detection of attack samples (Class 1).

Class imbalance issue affected recall for attack detection.

📈 Visualizations
Correlation Matrix Heatmap
Feature Importance (Random Forest)
Confusion Matrices for RF & SVM

⚡ How to Run the Code
1️⃣ Install Dependencies
pip install pandas numpy scikit-learn matplotlib seaborn
2️⃣ Run the Jupyter Notebook
Open cybersecurity_classification.ipynb

Run all cells to train models and generate results

🚀 Future Improvements
Use SMOTE to handle class imbalance  
Explore Deep Learning (e.g., Neural Networks)
Optimize SVM hyperparameters for better attack detection
