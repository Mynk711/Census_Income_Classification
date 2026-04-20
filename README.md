# Census Income Classification & Segmentation
## JPMC Take-Home Assessment

## Project Overview
This project builds a classification model to predict whether an individual earns above or below $50,000 annually, and a segmentation model to identify distinct customer groups for retail marketing purposes. The dataset is derived from the 1994-1995 US Census Bureau Current Population Surveys.

---

## Requirements

pandas
numpy
scikit-learn
matplotlib
seaborn
xgboost
joblib
statsmodels
jupyter
nbconvert
scipy

Install all dependencies:
pip install pandas numpy matplotlib seaborn scikit-learn xgboost joblib statsmodels jupyter nbconvert scipy

---

## How to Run

Option 1 - Run full pipeline:
python main.py

Option 2 - Run notebooks individually in order:
1. src/data_loader.ipynb — Load and explore raw data
2. src/preprocessing.ipynb — Clean data and create splits
3. src/feature_engineering.ipynb — Engineer features
4. src/train.ipynb — Train and tune models
5. src/evaluation.ipynb — Evaluate final model on test set
6. src/segmentation.ipynb — Build segmentation model

Note on Data Files:
The raw data files (census-bureau.data, census-bureau.csv) are excluded from this repository due to file size limits. Download them from the UCI Machine Learning Repository and place them in the data/ folder before running.

---

## Data
- Source: 1994-1995 US Census Bureau Current Population Surveys
- Size: 199,523 records, 42 features (196,294 after deduplication)
- Target: Binary income label (>$50k or <=$50k)
- Class imbalance: 6.2% positive class (>$50k)
- Population represented: ~347 million people via sampling weights

