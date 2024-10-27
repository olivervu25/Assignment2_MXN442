# MXN442 Assignment 2

**Author**: Thanh Long (Oliver) Vu  
**Student ID**: n11177071

This repository contains the implementation and replication of the paper:  
**Title**: *Data-Driven Subgroup Identification for Linear Regression*  
**Authors**: Zachary Izzo, Ruishan Liu, James Zou  
**DOI**: [10.48550/ARXIV.2305.00195](https://doi.org/10.48550/ARXIV.2305.00195)

## Repository Structure
```markdown

ASSIGNMENT2_MXN442/
│
├── data/
│   ├── Brazil_health.xls                # Dataset related to Brazil Health (Heart Failure, Stroke)
│   ├── China_glucose.xlsx               # Dataset related to China Glucose (SUA-F, SUA-M)
│   ├── China_HIV.dta                    # Dataset for China HIV
│   ├── Dutch_drinking.sav               # Dataset for Dutch Drinking
│   ├── Korea_grip.xlsx                  # Dataset for Korea Grip Strength
│   ├── Spain_Hair_Healthy.sav           # Dataset related to Spain Hair (Healthy group)
│   ├── Spain_Hair_Pregnancy.sav         # Dataset related to Spain Hair (Pregnancy group)
│
├── Result Images/
│   ├── Cluster_Region.png               # Visualization of regions from K-means clustering
│   ├── DDGroup_Region.png               # Visualization of regions from DDGroup model
│   ├── F1_Score_3Ms.png                 # F1 scores comparison between DDGroup, LMT, and K-means
│   ├── GBM_Region.png                   # Visualization of regions from GBM model
│   ├── LMT_Region.png                   # Visualization of regions from LMT model
│   ├── Precision_3Ms.png                # Precision comparison between DDGroup, LMT, and K-means
│   ├── Recall_3Ms.png                   # Recall comparison between DDGroup, LMT, and K-means
│   ├── SVM_Region.png                   # Visualization of regions from SVM model
│
├── utils/
│   ├── data_loader.py                   # Utility for loading datasets for model training and testing
│   ├── methods.py                       # Core methods for DDGroup, LMT, K-means
│
├── Models_with_Real_data.ipynb           # Notebook with experiments on real-world datasets
├── Models_with_Synthetic_data.ipynb      # Notebook with experiments on synthetic datasets
│
├── README.md                            # This file
└── requirements.txt                     # List of dependencies needed to run the notebooks.

```

## Requirements

To ensure smooth reproduction of the experiments and results, you will need the following software and packages installed:

- **Python version**: 3.10+
- **Packages**:
  - `numpy`
  - `scikit-learn`
  - `lineartree`
  - `matplotlib`
  - `tqdm`
  - `scipy`
  - `pandas`
  - `tabulate`
  - `pyreadstat`

## Instructions for Running

### Step 1: Install Dependencies
Make sure to install all required libraries before running the notebooks. You can do this by running the following command in your terminal:

```bash
pip install -r requirements.txt
```
### Step 2: Run the Notebooks

There are two main Jupyter notebooks you need to run:

1. **Models with Synthetic Data**  
   - **Location**: `Models_with_Synthetic_data.ipynb`
   - **Description**: This notebook replicates three models (DDGroup, LMT, and K-means clustering) and implements two new models (SVM and GBM) for synthetic data.
   - **Runtime**: It takes approximately 15-20 minutes to run. On a MacBook Pro M1 Pro 2021, it completes in around 15 minutes.

2. **Models with Real-World Data**  
   - **Location**: `Models_with_Real_data.ipynb`
   - **Description**: This notebook applies the DDGroup and GBM models to the five real-world datasets provided in the paper. Some datasets include 2-3 sub-datasets for more detailed analysis.
   - **Runtime**: This notebook takes around 5 minutes to complete.

### Step 3: Outputs

Both notebooks will generate output images and metrics, which are saved in the `Result Images` folder. These include figures for evaluating the models in terms of precision, recall, and F1 score.
