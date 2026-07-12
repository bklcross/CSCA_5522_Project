# Student Academic Risk Prediction

This project uses the [Student Performance dataset](https://www.kaggle.com/datasets/devansodariya/student-performance-data) to predict whether a student is academically at risk.

- At risk: `G3 < 10`
- Not at risk: `G3 >= 10`

It compares Logistic Regression, Decision Tree, Random Forest, and Gradient Boosting with two feature sets: one including `G1` and `G2`, and one excluding them for earlier prediction. Models are evaluated with accuracy, precision, recall, F1, and a confusion matrix, with recall treated as the primary metric.

## Setup

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

## Run

```bash
jupyter notebook student_risk_project.ipynb
```

The notebook downloads the dataset with KaggleHub. To use a local CSV instead,
set `CSV_PATH` in the dataset-loading cell.

## Outputs

The `outputs/` directory contains:

- `data_overview.png`
- `model_results.csv`
- `confusion_matrix.png`
- `feature_importance.csv` and `.png`
