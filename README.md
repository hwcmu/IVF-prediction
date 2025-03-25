# Predicting IV Fluid Utilization in Emergency Departments  
**Integrating Structured and Unstructured Clinical Data with NLP and Machine Learning**

This repository contains the complete code, data, and results for a study aimed at predicting intravenous (IV) fluid utilization in emergency department (ED) settings using a multimodal approach. Structured clinical data is combined with unstructured patient narratives processed using GPT-2 embeddings.

---

## Repository Structure
├── ed_data.csv # Raw dataset 

├── text cleaning.ipynb # NLP preprocessing pipeline 
├── data_before_model.ipynb # Structured + unstructured data preparation 
│ ├── cleaned_ed_data.csv # dataset after text cleaning dataset 


├── descriptive analysis.ipynb # Exploratory data analysis 
│ ├── descriptive_results.pkl # Summary stats from EDA 

├── Base LR.ipynb # Logistic Regression model notebook 
├── GBC.ipynb # Gradient Boosting Classifier model notebook 

├── Figure 1. Forest Plot of ORs.png # Visual: Odds Ratios from Logistic Regression 
├── Figure 2. Mean ROC curve.jpg # Visual: ROC curve for model comparison 
├── README.md # This file
