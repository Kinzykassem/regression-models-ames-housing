# Regression Models — Ames Housing 🏠📊

A practical machine-learning training exercise focused on regression models and house-price prediction using the Ames Housing dataset.

## 🚀 Live Demo

👉 **[Try the Ames House Price Predictor](https://regression-models-ames-housing.streamlit.app/)**

Use the interactive Streamlit application to enter house features and get an estimated sale price from the trained Ridge Regression model.

## 📌 Context

This repository contains my practical work from regression-models training at the Arab Academy for Science, Technology & Maritime Transport.

The notebook covers data exploration, preprocessing, several regression algorithms, model evaluation, model comparison, and saving trained models for prediction.

## 🤖 Models Explored

- Simple Linear Regression
- Multiple Linear Regression
- Polynomial Regression
- Ridge Regression
- Lasso Regression
- Elastic Net
- Support Vector Regression (SVR)
- Decision Tree Regression
- Random Forest Regression

## 📈 Model Comparison

| Model | MAE | RMSE | R² |
|---|---:|---:|---:|
| Ridge | $13,829 | $22,230 | 0.930 |
| Lasso | $13,905 | $21,661 | 0.934 |
| Elastic Net | $13,905 | $21,661 | 0.934 |
| Random Forest | $14,217 | $22,342 | 0.930 |
| Polynomial | $14,422 | $24,002 | 0.919 |
| Multiple Linear | $15,392 | $23,701 | 0.921 |
| SVR | $15,396 | $22,674 | 0.928 |
| Decision Tree | $19,285 | $28,036 | 0.889 |
| Simple Linear | $39,604 | $58,520 | 0.518 |

Lasso and Elastic Net achieved the highest R² of **0.934**, while Ridge achieved the lowest MAE.

For the interactive application, Ridge Regression is used with a complete preprocessing + model pipeline.

## 📁 Project Structure

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

## 💻 Run Locally

```bash
pip install -r requirements.txt
python -m streamlit run app.py

## 📓 Training Notebook

The main notebook is `regression.ipynb`, which contains the practical analysis, preprocessing steps, model experiments, evaluation, and comparison.

## 📊 Example Prediction

The trained Ridge model was used to estimate the price of a new house based on its features.

**Estimated sale price: approximately $210K**

## ⚠️ Notes

- The dataset is the Ames Housing dataset used for the training exercise.
- The saved Ridge model expects the same raw feature names used in the notebook.
- The application is intended as an educational demonstration, not as a professional real-estate valuation tool.

## 🔗 Links

- **GitHub:** https://github.com/Kinzykassem/regression-models-ames-housing
- **Live Streamlit App:** https://regression-models-ames-housing.streamlit.app/
