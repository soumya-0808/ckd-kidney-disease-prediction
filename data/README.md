# Dataset

The repository contains the supplied `kidney_disease.csv` under `data/raw/`.

The project materials describe the data as a 400-record Chronic Kidney Disease clinical dataset originally associated with the UCI CKD dataset and accessed through a Kaggle notebook. The supplied paper identifies the Kaggle source as the `Chronic Kidney Disease` notebook by Nitesh Yadav. See the paper and thesis in `docs/` for the project's source description.

## Files

- `raw/kidney_disease.csv`: supplied 400 × 26 tabular dataset.
- `processed/final_intersection_dataset.csv`: the 7-feature intersection used by the supplied feature-selection notebook, plus the target.

## Target

`classification` is the binary target used in the supplied dataset:

- `1` = CKD
- `0` = Non-CKD

This mapping follows the project materials and dataset values. The dataset contains missing clinical values and mixed numeric/categorical columns, so preprocessing is required before model training.

## Medical-data note

This repository is an academic machine-learning project, not a clinical diagnostic system. It should not be used to make medical decisions.
