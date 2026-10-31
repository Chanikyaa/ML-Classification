# Classical Machine Learning Classification

A machine learning classification project using the Wine dataset to train, evaluate, and compare classification models with a reproducible evaluation workflow.

## Overview

This project demonstrates a complete classical machine learning workflow, from data preparation and model training to evaluation and regression checks.

The implementation uses the Wine dataset and evaluates a logistic regression classifier against a majority-class baseline.

## Key Features

- Dataset loading and preprocessing.
- Classification model training.
- Logistic regression.
- Majority-class baseline comparison.
- Accuracy evaluation.
- Macro-F1 evaluation.
- Model performance regression gate.
- Automated testing.

## Dataset

The project uses the Wine classification dataset, a commonly used dataset for multi-class classification.

The dataset contains chemical measurements used to predict wine classes.

## Machine Learning Workflow

```text
          Wine Dataset
                |
                v
        Data Preparation
                |
                v
          Train / Test Split
                |
                v
         Model Training
                |
         +------+------+
         |             |
         v             v
    Logistic       Majority-Class
   Regression        Baseline
         |             |
         +------+------+
                |
                v
         Model Evaluation
                |
                v
       Accuracy / Macro-F1
                |
                v
       Performance Gate
```

## Technology Stack

- Python
- Scikit-learn
- Pandas
- NumPy
- Pytest
- MLflow (optional)

## Project Structure

```text
classical-ml-classification/
│
├── src/
├── data/
├── models/
├── tests/
├── requirements.txt
├── README.md
└── .gitignore
```

*Use the actual project tree when documenting the repository.*

## Installation

```bash
git clone https://github.com/Chanikyaa/classical-ml-classification.git
cd classical-ml-classification

python -m venv .venv
```

Activate the environment:

**Windows**
```bash
.venv\Scripts\activate
```

**Linux/macOS**
```bash
source .venv/bin/activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

## Running the Project

Run the training and evaluation workflow using the entry point provided in the project source code.

Refer to the repository instructions for the exact command.

## Evaluation Results

<text>Reported results from the included test split:</text>

| Metric | Logistic Regression | Majority Baseline |
|---|---:|---:|
| Accuracy | 0.9722 | 0.3889 |
| Macro-F1 | 0.9710 | 0.1867 |

- Test observations: **36**
- Macro-F1 regression threshold: **0.80**
- Regression gate: **Passed**

These results apply to the included split and should not be interpreted as a guarantee of performance on new datasets.

## Testing

```bash
pytest
```

## Current Validation

- Automated tests: **8 passed**.
- Clean ZIP extraction test: **8 passed**.
- Python editable installation was not verified because dependency installation required network access that was unavailable.
- Optional MLflow integration was not exercised.
- Docker and hosted CI have not been verified.

## Engineering Concepts Demonstrated

- Supervised machine learning
- Multi-class classification
- Data preprocessing
- Baseline comparison
- Model evaluation
- Macro-F1
- Performance regression testing
- Reproducible experiments

## Future Improvements

- Add cross-validation.
- Compare multiple classification algorithms.
- Add hyperparameter optimization.
- Track experiments with MLflow.
- Add explainability with SHAP.
- Build a model prediction API.

## Author

**Palli Chanikya Paidi Balaji**

B.Tech – VIT Chennai (2025)  
M.Tech CSE – AI & Data Science, Mahindra University (2026–2028)

GitHub: [@Chanikyaa](https://github.com/Chanikyaa)

---

*Part of an AI/ML Engineering Portfolio.*
