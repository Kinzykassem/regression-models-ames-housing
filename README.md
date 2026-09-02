# Regression Models — Ames Housing

A practical machine-learning training exercise focused on regression models and house-price prediction using the Ames Housing dataset.

## Context

This repository contains my practical work from regression-models training at the Arab Academy for Science, Technology & Maritime Transport.

The notebook covers data exploration, preprocessing, several regression algorithms, model evaluation, comparison, and saving trained models for prediction.

## Models explored

- Simple Linear Regression
- Multiple Linear Regression
- Polynomial Regression
- Ridge Regression
- Lasso Regression
- Elastic Net
- Support Vector Regression (SVR)
- Decision Tree Regression
- Random Forest Regression

## Best results

| Model | MAE | RMSE | R² |
|---|---:|---:|---:|
| Ridge | $13,829 | $22,230 | 0.930 |
| Lasso | $13,905 | $21,661 | 0.934 |
| Elastic Net | $13,905 | $21,661 | 0.934 |
| Random Forest | $14,217 | $22,342 | 0.930 |
| Polynomial | $14,422 | $24,002 | 0.919 |
| SVR | $15,396 | $22,674 | 0.928 |
| Multiple Linear | $15,392 | $23,701 | 0.921 |
| Decision Tree | $19,285 | $28,036 | 0.889 |
| Simple Linear | $39,604 | $58,520 | 0.518 |

For the interactive app, Ridge Regression is used because it provides a strong balance of performance and stability, and the saved model is a complete preprocessing + model pipeline.

## Project structure

```text
regression-models-ames-housing/
├── regression.ipynb
├── app.py
├── requirements.txt
├── README.md
├── data/
│   └── ames.csv
└── models/
    └── 04_ridge.joblib
```

## Run locally

```bash
pip install -r requirements.txt
streamlit run app.py
```

## Streamlit App

After deployment, add the public Streamlit URL here.

## Training notebook

The main notebook is `regression.ipynb`, which contains the practical analysis and model experiments.

## Notes

- The dataset is the Ames Housing dataset used for the training exercise.
- The saved Ridge model expects the same raw feature names used in the notebook.
- The application is intended as an educational demonstration, not as a professional real-estate valuation tool.
