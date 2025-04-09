# Predicting IV Fluid Utilization in Emergency Departments  
**Integrating Structured and Unstructured Clinical Data with NLP and Machine Learning**

---

## Description  
This repository contains the full code, data, and results for a project that predicts intravenous (IV) fluid utilization in emergency departments (EDs) using both structured and unstructured clinical data. Unstructured patient narratives are processed via GPT-2 embeddings, while machine learning models—specifically logistic regression and gradient boosting—are used for prediction. The study is reproducible in Google Colab for ease of access and verification.

---

## Dataset Information  
- **Source**: 2021 National Hospital Ambulatory Medical Care Survey – Emergency Department (NHAMCS-ED)  
- **Access**:  
  - [CDC NHAMCS Documentation](https://www.cdc.gov/nchs/ahcd/index.htm)  
  - [Survey Descriptions & Codebooks](https://ftp.cdc.gov/pub/Health_Statistics/NCHS/dataset_documentation/nhamcs/)  
  - [Raw SAS Data](https://ftp.cdc.gov/pub/Health_Statistics/NCHS/Datasets/NHAMCS/)  
  - [SAS Format Files](https://ftp.cdc.gov/pub/Health_Statistics/NCHS/dataset_documentation/nhamcs/sas/)  

> **Note**: All data used are publicly available and anonymized. No ethical review or participant consent was required.

---

## Repository Structure  

- `README.md` – Project overview, setup, and usage guide  
- `ed_data.csv` – Raw dataset from NHAMCS-ED 2021  
- **Notebooks**:  
  - `text cleaning.ipynb` – Processing unstructured notes  
  - `data_before_model.ipynb` – Data merging and feature engineering  
  - `descriptive analysis.ipynb` – Summary statistics and visualizations  
  - `Base LR.ipynb` – Logistic Regression modeling  
  - `GBC.ipynb` – Gradient Boosting Classifier modeling  
- **Supplementary Files**:  
  - `cleaned_ed_data.csv`, `processed_data.7z` – Preprocessed datasets  
  - `Figure 1. Forest Plot of ORs.png`, `Figure 2. Mean ROC curve.jpg` – Visualizations of results  

---

## Usage Instructions  

1. Open notebooks in Google Colab or your local Jupyter environment.  
2. Start with `text cleaning.ipynb` to process raw text data.  
3. Proceed through the modeling notebooks in order (`data_before_model.ipynb` → `Base LR.ipynb` / `GBC.ipynb`).  
4. Visualizations and performance metrics are generated at each step.  

---

## Requirements  

Ensure the following libraries are installed (automatically handled in Colab):  
```bash
pandas  
numpy  
scikit-learn  
matplotlib  
seaborn  
transformers  
joblib  
```

---

## Methodology  

- **Data Processing**: Combined structured data (vitals, diagnoses) with unstructured ED visit narratives.  
- **Text Embedding**: GPT-2 embeddings used for representing clinical narratives.  
- **Modeling**:  
  - Logistic Regression (baseline)  
  - Gradient Boosting Classifier (GBC)  
- **Evaluation**: ROC curves, feature importance (OR plots), and cross-validation for model comparison.

---

## Declarations  

- **Human Ethics and Consent to Participate**: Not applicable, as this study utilized publicly available, anonymized data from the NHAMCS-ED dataset.  
- **Consent to Participate**: Not applicable.  
- **Ethics Approval**: Not applicable.  
- **Funding**: This research received no specific grant from any funding agency, commercial, or not-for-profit sectors.  
- **Availability of Data and Material**:  
  - Data are available via the CDC: https://www.cdc.gov/nchs/ahcd/index.htm  
  - Survey documentation and codebooks: https://ftp.cdc.gov/pub/Health_Statistics/NCHS/dataset_documentation/nhamcs/  
  - SAS datasets: https://ftp.cdc.gov/pub/Health_Statistics/NCHS/Datasets/NHAMCS/  
  - SAS format files: https://ftp.cdc.gov/pub/Health_Statistics/NCHS/dataset_documentation/nhamcs/sas/  
- **Competing Interests**: The authors declare that they have no competing interests.
