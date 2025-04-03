## Predicting IV Fluid Utilization in Emergency Departments: Integrating Structured and Unstructured Clinical Data with NLP and Machine Learning

This repository contains the complete code, data, and results for a study aimed at predicting intravenous (IV) fluid utilization in emergency department (ED) settings using a multimodal approach. The project combines structured clinical data with unstructured patient narratives processed using GPT-2 embeddings, and leverages machine learning techniques to enhance predictive performance. All experiments and analyses are designed to be fully reproducible in a Google Colab environment, ensuring easy access and execution for researchers and practitioners.

### Repository Structure and Reproducibility
The repository is organized to facilitate clear navigation and reproducibility. Key files and directories include:

- README.md: This file, which provides an overview of the project, instructions for setup, and detailed explanations of each component.

- ed_data.csv: The raw dataset sourced from the 2021 National Hospital Ambulatory Medical Care Survey – Emergency Department (NHAMCS-ED).

- Notebooks such as text cleaning.ipynb, data_before_model.ipynb, descriptive analysis.ipynb, Base LR.ipynb, and GBC.ipynb that outline the full data processing pipeline, exploratory analysis, and model building for both logistic regression and Gradient Boosting Classifier.

- Supplementary files, including preprocessed datasets (cleaned_ed_data.csv, processed_data.7z) and visual outputs (Figure 1. Forest Plot of ORs.png, Figure 2. Mean ROC curve.jpg), provide detailed insights into the data and model performance.
This structured approach, coupled with step-by-step instructions in the Colab notebooks, ensures that the experiments can be replicated easily by anyone with access to a Google Colab account.
