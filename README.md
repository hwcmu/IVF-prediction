# Integrating multimodal clinical data to predict intravenous (IV) fluid utilization

Reproducibility repository for the published open-access article:

> Wang, H., Ling, H., & Zhang, X. (2025). Integrating multimodal clinical data to predict intravenous (IV) fluid utilization: a comparative analysis of natural language processing techniques. *PeerJ Computer Science*, 11, e3441. https://doi.org/10.7717/peerj-cs.3441

## Quick Links

- Published article: https://peerj.com/articles/cs-3441
- DOI: https://doi.org/10.7717/peerj-cs.3441
- Repository: https://github.com/hwcmu/IVF-prediction

## Repository Scope

This repository contains code, data-processing notebooks, and generated figures
for predicting intravenous (IV) fluid utilization in emergency department visits
using structured clinical variables and unstructured patient narratives.

The published article evaluates multimodal models using the 2021 National
Hospital Ambulatory Medical Care Survey Emergency Department dataset
(NHAMCS-ED, n = 13,115). Text features are derived from patient narratives using
several NLP representations, and the structured and unstructured features are
combined before model fitting.

## Main Findings Reflected in This Repository

- Multimodal models using structured variables plus patient narratives
  outperformed models using either data source alone.
- Traditional frequency-based NLP features, especially CountVectorizer,
  performed strongly for short emergency-department complaint text.
- Gradient Boosting and Logistic Regression were used as the main supervised
  learning models in the analysis workflow.

## Data

- Source: 2021 NHAMCS-ED public-use data.
- Access:
  - CDC NHAMCS documentation: https://www.cdc.gov/nchs/ahcd/index.htm
  - Codebooks and documentation: https://ftp.cdc.gov/pub/Health_Statistics/NCHS/dataset_documentation/nhamcs/
  - Raw SAS data: https://ftp.cdc.gov/pub/Health_Statistics/NCHS/Datasets/NHAMCS/

The repository uses public, anonymized survey data. No individual-level private
clinical records are included.

## Files

- `text cleaning.ipynb`: processing for unstructured patient narratives.
- `data_before_model.ipynb`: data merging and feature engineering.
- `descriptive analysis.ipynb`: summary statistics and visualizations.
- `model comparison embedding.py`: model comparison workflow for text embeddings.
- `ed_data.csv`: NHAMCS-ED 2021 input data used in the workflow.
- `cleaned_ed_data.csv`: processed analysis data.
- `Figure 1 pipeline.png`, `Figure 2 heatmap_differences.png`,
  `Figure 3. Forest Plot of Odds Ratios with 95% CI (Log Scale).png`,
  `Figure 4 lr_roc.png`, `Figure 5 gbc_roc.png`: generated analysis figures.

## Citation

```bibtex
@article{wang2025ivfluid,
  title = {Integrating multimodal clinical data to predict intravenous (IV) fluid utilization: a comparative analysis of natural language processing techniques},
  author = {Wang, Hairong and Ling, Haipeng and Zhang, Xingyu},
  journal = {PeerJ Computer Science},
  volume = {11},
  pages = {e3441},
  year = {2025},
  doi = {10.7717/peerj-cs.3441},
  url = {https://doi.org/10.7717/peerj-cs.3441}
}
```

