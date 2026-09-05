# Homework 0 — Warm-Up Exercises

Ungraded lead-in exercises from the start of the course: getting comfortable with Jupyter/Markdown, refreshing NumPy fundamentals, and working through a full regression project end to end before diving into neural networks proper.

## Contents

| File | Description |
|---|---|
| `c_markup_summary.ipynb` | Notes on Jupyter Notebook basics and Markdown syntax used for documenting later assignments. |
| `e_numpy_boardcasting.ipynb` | NumPy broadcasting exercises — array creation, shape rules, and vectorized operations. |
| `g_math_practice.ipynb` | Linear algebra/calculus refresher — vectors, matrix ops, gradients, chain rule, gradient descent, softmax. *(Added later — this notebook was empty in the original coursework; see root [Known Gaps](../README.md#known-gaps).)* |
| `d_f_car_resale_val_prediction_end2endproj/` | An end-to-end regression project predicting car resale value, following the classic Géron *Hands-On Machine Learning* workflow (EDA → feature prep → model selection). |

## Car Resale Value Prediction

`d_f_car_resale_val_prediction_end2endproj/car_resale_val_prediction.ipynb` walks through:

- Loading and exploring `Car_sales.csv` (manufacturer, price, engine specs, etc.)
- Exploratory data analysis with histograms and scatter matrices (saved under `images/end_to_end_project/`)
- Data cleaning and feature preparation with `scikit-learn`
- Training and evaluating regression models to predict resale value

This one predates the deep learning portion of the course — it's classical ML (pandas/scikit-learn), included here as the foundation the rest of the coursework builds on.

## Run it

Install from [`requirements.txt`](requirements.txt) (NumPy, pandas, matplotlib, seaborn, scikit-learn, SymPy).
