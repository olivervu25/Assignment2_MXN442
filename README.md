# MXN442 Assignment 2

**Author**: Thanh Long (Oliver) Vu  
**Student ID**: n11177071

This repository contains the implementation and replication of the paper:  
**Title**: *Data-Driven Subgroup Identification for Linear Regression*  
**Authors**: Zachary Izzo, Ruishan Liu, James Zou  
**DOI**: [10.48550/ARXIV.2305.00195](https://doi.org/10.48550/ARXIV.2305.00195)

## Repository Structure

## Repository Structure

├── Replication/
│   ├── F1_Score_3Ms.png   # F1 scores for DDGroup, LMT, and Clustering models
│   ├── Precision_3Ms.png  # Precision scores for DDGroup, LMT, and Clustering models
│   ├── Recall_3Ms.png     # Recall scores for DDGroup, LMT, and Clustering models
│   ├── F1_Score_4Ms.png   # F1 scores for all 4 models including XGBoost
│   ├── Precision_4Ms.png  # Precision scores for all 4 models including XGBoost
│   ├── Recall_4Ms.png     # Recall scores for all 4 models including XGBoost
│
├── utils/
│   ├── data_loader.py      # Helper script for loading datasets
│   ├── methods.py          # Methods for various model implementations, including DDGroup
│
├── New Method/
│   ├── F1_Score_XGB.png   # F1 scores for new XGBoost method
│   ├── Precision_XGB.png  # Precision scores for new XGBoost method
│   ├── Recall_XGB.png     # Recall scores for new XGBoost method
│
├── performance_vs_n.ipynb # Main notebook for running experiments, includes results and visualizations
└── README.md              # This readme file


## Requirements

To ensure smooth reproduction of the experiments and results, you will need the following software and packages installed:

- **Python version**: 3.10+
- **Packages**:
  - `numpy`
  - `scikit-learn`
  - `xgboost`
  - `matplotlib`
  - `tqdm`
  - `seaborn`
  - `pandas`

## Repository Structure

.
├── Replication/
│   ├── F1_Score_3Ms.png          # F1 scores for DDGroup, LMT, and Clustering models
│   ├── Precision_3Ms.png         # Precision scores for DDGroup, LMT, and Clustering models
│   ├── Recall_3Ms.png            # Recall scores for DDGroup, LMT, and Clustering models
│   ├── F1_Score_4Ms.png          # F1 scores for all 4 models including XGBoost
│   ├── Precision_4Ms.png         # Precision scores for all 4 models including XGBoost
│   ├── Recall_4Ms.png            # Recall scores for all 4 models including XGBoost
│
├── utils/
│   ├── data_loader.py            # Helper script for loading datasets
│   ├── methods.py                # Methods for various model implementations, including DDGroup
│
├── New Method/
│   ├── F1_Score_XGB.png          # F1 scores for new XGBoost method
│   ├── Precision_XGB.png         # Precision scores for new XGBoost method
│   ├── Recall_XGB.png            # Recall scores for new XGBoost method
│
├── performance_vs_n.ipynb        # Main notebook for running experiments, includes results and visualizations
└── README.md                     # This readme file


## Instructions for Running

