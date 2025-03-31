# 💳 Credit Card Fraud Detection using Machine Learning  

## 📌 Project Overview  
Fraudulent credit card transactions pose a significant risk to financial institutions and customers, leading to financial losses and reputational damage. This project leverages machine learning to build a fraud detection system that accurately identifies fraudulent transactions while minimizing false positives.  

## 🔍 Dataset Overview  
- Source: [Kaggle - Credit Card Fraud Detection](https://www.kaggle.com/mlg-ulb/creditcardfraud)  
- Transactions: **284,807** (European cardholders over two days in September 2013)  
- Fraudulent Transactions: **492** (~0.172% of total)  
- Features:  
  - **V1–V28:** Principal components derived using PCA  
  - **Time:** Seconds elapsed since the first transaction  
  - **Amount:** Transaction amount  
  - **Class:** Target variable (1 = Fraud, 0 = Legitimate)  
- **Challenge:** Highly imbalanced dataset requiring specialized handling techniques.  

## 🛠️ Methodology  
1. **Data Preprocessing:**  
   - Handled missing values  
   - Standardized features  
   - Addressed class imbalance using oversampling techniques (Random Oversampling, SMOTE, ADASYN)  

2. **Exploratory Data Analysis (EDA):**  
   - Examined class distributions and feature correlations  
   - Identified dataset imbalance and its impact  

3. **Model Training & Evaluation:**  
   - Implemented multiple machine learning models:  
     - Logistic Regression  
     - Decision Tree  
     - Random Forest  
     - XGBoost  
   - Evaluated performance using key classification metrics:  
     - **ROC-AUC Score**  
     - **Precision, Recall, and F1-Score**  
     - **Confusion Matrix Analysis**  

## 📊 Performance Summary  
- **XGBoost (Random Oversampling) emerged as the best-performing model** based on the **ROC-AUC score**.  
- This model achieved:  
  - **High Precision (~90%)** ensuring minimal false positives.  
  - **Strong Recall (~86%)** capturing fraudulent transactions effectively.  
  - **Highest F1-Score** among all models, balancing precision and recall optimally.  

## 🚀 Key Takeaways  
✅ Machine learning significantly improves fraud detection accuracy.  
✅ Handling class imbalance is critical—oversampling techniques enhanced model performance.  
✅ Feature scaling and PCA-transformed variables played a crucial role in improving predictions.  

## 📌 Future Enhancements  
🔹 Experiment with deep learning models (e.g., LSTMs for sequential fraud detection).  
🔹 Fine-tune hyperparameters further for performance gains.  
🔹 Deploy the model as an API for real-time fraud detection.  

## 🛠️ Tech Stack  
- **Languages & Libraries:** Python, Pandas, NumPy, Scikit-Learn, XGBoost, Matplotlib, Seaborn  
- **Machine Learning Techniques:** Classification, PCA, Oversampling (SMOTE, ADASYN)  
- **Model Evaluation Metrics:** ROC-AUC, Precision, Recall, F1-Score
- 
