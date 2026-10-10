# Value-Optimized ML for Small-Farm Crop Classification

University machine-learning project on cost-aware classification of dry beans using morphology measurements.

## Overview

This project evaluates whether a crop-classification model can stay accurate while requiring far fewer physical measurements. The dataset contains **13,611 dry-bean samples** across **7 varieties** with **16 morphology features**.

The goal was not only to maximize accuracy, but to find a practical tradeoff between model performance and the cost/effort of collecting measurements.

## Approach

Models compared:

- Logistic Regression
- Decision Tree
- Random Forest
- Dense Neural Network

After benchmarking the models, I designed a cost-to-accuracy feature-selection strategy to identify which small subsets of measurements preserved the most predictive value.

## Key result

The feature-selection strategy reduced required measurements by **69–81%** — from **16 features down to 3–5 features** — while preserving **98.4–98.7% of the full-feature Random Forest accuracy**.

That result is the point of the project: near-baseline predictive performance with a much cheaper measurement process.

## Repository contents

- `Optimizing_Dry_Bean_Classification.ipynb` — main analysis notebook with model training, evaluation, and feature-selection experiments.
- `DryBeanDataset/` — dataset files used by the notebook.
- `Resources/` — supporting project materials.
- `ML_Project_Proposal_Finalized.pptx` — original project proposal deck.

## Tech stack

Python · Pandas · NumPy · scikit-learn · TensorFlow/Keras · Jupyter Notebook

## How to review

Open `Optimizing_Dry_Bean_Classification.ipynb` and read from top to bottom: data loading and exploration, baseline model comparison, feature-importance/feature-subset analysis, then final tradeoff results.

## Notes

Academic project completed at UTEP in Spring 2026. Results should be interpreted within the dataset and experimental setup in the notebook.
