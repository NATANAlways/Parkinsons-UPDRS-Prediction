# Parkinson’s UPDRS Prediction using Bioinformatics Approaches

**Author:** S. Nathiskar 

## Overview

This project analyzes the **Parkinson’s Telemonitoring Dataset** from the UCI Machine Learning Repository to predict **UPDRS (Unified Parkinson’s Disease Rating Scale)** scores. The notebook demonstrates how voice-based acoustic features and patient metadata can be used to model Parkinson’s disease progression.

The workflow covers:

* Exploratory Data Analysis (EDA)
* Data cleaning and preprocessing
* Feature analysis and engineering
* Regression model training and evaluation

## Dataset

* **Source:** [UCI Parkinson’s Telemonitoring Data](https://archive.ics.uci.edu/dataset/189/parkinsons+telemonitoring)
* **Samples:** 5,875
* **Features:** 22 acoustic and clinical features (e.g., Jitter, Shimmer, NHR, HNR, PPE, etc.)
* **Targets:**

  * `motor_UPDRS` – Motor function score
  * `total_UPDRS` – Total score (used in this lab)

## Objectives

1. Load and explore dataset structure
2. Understand and describe feature types and targets
3. Preprocess data (cleaning, scaling, train-test split)
4. Train baseline regression models (e.g., Linear Regression, Ridge, Lasso, Random Forest)
5. Evaluate models using MAE, RMSE, and R² metrics

## Repository Structure

```
.
├── 2021E190_Lab02.ipynb   # Main analysis notebook
└── parkinsons_updrs.data.csv   # Dataset
```

## Tools & Libraries

* Python 3.x
* Pandas, NumPy
* Matplotlib, Seaborn (visualization)
* Scikit-learn (modeling & evaluation)
* Jupyter Notebook

## Quick Start

```bash
# 1. Clone the repository
git clone https://github.com/<your-username>/Parkinsons-UPDRS-Prediction.git
cd Parkinsons-UPDRS-Prediction

# 2. Create and activate environment (optional)
python -m venv .venv
source .venv/bin/activate   # Linux/Mac
.venv\Scripts\activate      # Windows

# 3. Install dependencies
pip install -r requirements.txt

## Results

* Baseline regression models trained to predict `total_UPDRS`.
* Feature correlations explored (e.g., strong correlation between some jitter/shimmer measures and UPDRS).
* Performance evaluated using regression metrics.

## References

* Tsanas et al., *Accurate telemonitoring of Parkinson’s disease progression by noninvasive speech tests*, IEEE Biomedical Engineering, 2010.
* UCI Machine Learning Repository – Parkinson’s Telemonitoring Data.
