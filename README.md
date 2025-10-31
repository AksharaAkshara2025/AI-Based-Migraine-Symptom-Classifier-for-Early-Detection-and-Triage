# AI-Based Migraine Symptom Classifier for Early Detection and Triage

## Overview
Migraines affect over one billion people worldwide and occur in multiple subtypes such as *migraine with aura*, *without aura*, *chronic*, and *hemiplegic* forms.  
Delayed or incorrect diagnosis often leads to poor treatment outcomes.

This project, developed under **NeuroHealthTech’s digital health initiative**, builds a **machine learning-based migraine classifier** to support early detection and triage in clinical settings.  
Using structured symptom data, the model predicts the migraine type based on patient-reported features.

---

## Dataset Description
- **Source:** [Kaggle – Migraine Symptom Dataset for Classification](https://www.kaggle.com/datasets/gzdekzlkaya/migraine-symptom-dataset-for-classification)  
- **Author:** *Gözde Kızılkaya*  
- **Records:** ~2000 entries  
- **Format:** CSV  
- **License:** Open for research and non-commercial use  

### Key Features:
- **Demographics:** Age, Attack Duration, Frequency  
- **Pain Attributes:** Location (Unilateral, Bilateral, Frontal, Temporal), Character (Throbbing, Pressing, Sharp, Dull), Intensity (1–5)  
- **Neurological & Systemic Symptoms:** Nausea, Vomit, Photophobia, Phonophobia, Visual, Sensory, Motor, Vertigo, Tinnitus, etc.  
- **Target Variable:** Type of migraine  
  - Migraine without aura  
  - Migraine with aura  
  - Chronic migraine  
  - Hemiplegic migraine  
  - Retinal migraine  

---

## Workflow
1. **Exploratory Data Analysis (EDA)**  
   - Visualize class distributions and relationships between features.  
   - Identify key symptoms contributing to each migraine subtype.

2. **Data Preprocessing**  
   - Encode categorical features and scale numeric variables.  
   - Handle missing data and class imbalance using SMOTE.  

3. **Model Building**  
   - Train baseline models: Logistic Regression, Decision Tree, Random Forest.  
   - Test advanced models: XGBoost, LightGBM, or Neural Networks.  
   - Tune hyperparameters for optimal performance.  

4. **Model Evaluation**  
   - Evaluate performance using Accuracy, F1-Score, and Confusion Matrix.  
   - Use SHAP for explainable AI to visualize feature importance.  

5. **Streamlit Deployment**  
   - Build a simple web interface for real-time symptom input and prediction.  

---

## Tools & Libraries
- **Programming Language:** Python 
- **Core Libraries:** Pandas, NumPy, Scikit-learn  
- **Visualization:** Matplotlib, Seaborn, Plotly  
- **Advanced ML:** XGBoost, LightGBM  
- **Explainability:** SHAP  
- **Deployment:** Streamlit 
- **Model Persistence:** joblib / pickle  

---

## Results & Insights
- **Best Models:** Random Forest and XGBoost delivered the highest accuracy and balanced performance across migraine classes.  
- **Top Predictors:** Visual disturbances, Pain Intensity, and Photophobia were among the most influential symptoms.  
- **Interpretability:** SHAP analysis provided clear insights into how each feature impacts prediction outcomes.  

**Outcome:**  
A robust, interpretable, and data-driven migraine classification model demonstrating how AI can enhance healthcare diagnostics and triage.

---
