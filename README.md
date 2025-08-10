# 💧 Water Potability Prediction for SDG 6: Clean Water and Sanitation

## 📌 Project Overview
Access to safe drinking water is a significant global challenge, directly linked to **United Nations Sustainable Development Goal 6** (Clean Water and Sanitation).  
This project uses **Machine Learning** to predict whether a given water sample is **potable (safe for consumption)** based on its physicochemical attributes such as pH, hardness, chloramines, and solids.  

The aim is to provide an automated, data‑driven method to help prioritize water testing and treatment.

---

## 🎯 Problem Statement
Traditional water quality testing can be **costly and time‑consuming**.  
By leveraging ML, we can predict water safety quickly and at scale — enabling **faster decision-making** for public health agencies and communities.

---

## 🔍 Process & Methodology
1. **Data Acquisition & Understanding**
   - Dataset: Publicly available CSV file containing water quality measurements and potability labels (0 = Not Potable, 1 = Potable).
   - Verified data quality and checked for missing values.
   
2. **Data Preprocessing**
   - Split data into training (80%) and test (20%) sets.
   - Applied `StandardScaler` for models sensitive to feature scale (e.g., KNN).

3. **Model Training & Evaluation**
   - Implemented and compared:
     - Logistic Regression
     - Decision Tree
     - K‑Nearest Neighbors (KNN)
     - Random Forest
   - Hyperparameter tuning for Random Forest using **GridSearchCV** with 5‑fold cross‑validation.
   - Evaluated with Accuracy, ROC AUC, Precision, Recall, and F1‑score.

4. **Visualization**
   - Plotted **all Confusion Matrices** side‑by‑side.
   - Compared **all ROC curves** on a single plot.
   - Generated a metrics summary table.

---

## 📊 Results
- **Best Model:** Tuned Random Forest
- **Accuracy:** ~79%  
- **ROC AUC:** ~0.84  
- **Top Features:** pH, chloramines, and solids were the most important indicators for potability.

  <img width="728" height="363" alt="Screenshot 2025-08-11 023434" src="https://github.com/user-attachments/assets/367fe87e-42cb-4fba-bc93-78c178e43d82" />
  <img width="1714" height="885" alt="Screenshot 2025-08-11 023645" src="https://github.com/user-attachments/assets/c2323021-8c57-4128-a307-a2e4e22e7933" />


