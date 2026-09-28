# Project Overview

## Research objective

The supplied thesis describes the objective as developing and evaluating computational models for early CKD prediction using clinical datasets. It covers missing-data handling, outlier treatment, feature selection, multiple ML algorithms, an ensemble model, and a hybrid 1D CNN + KNN model.

## Dataset

The supplied research materials describe a 400-record CKD dataset with clinical and laboratory variables. The feature table in the conference paper identifies variables including serum creatinine, blood urea, hemoglobin, packed cell volume, random blood glucose, specific gravity, albumin, diabetes mellitus, hypertension, red blood cells, pus cells, sodium, potassium, white blood cell count, and red blood cell count.

## Feature selection

The supplied feature-selection notebook implements:

- Filter selection using ANOVA F-test / `SelectKBest`
- Wrapper selection using RFE + Logistic Regression
- Embedded selection using Random Forest feature importance
- Intersection of the three selected feature sets

The recorded intersection is `hemo`, `sg`, `htn`, `rbc`, `id`, `bgr`, and `al`.

## Model tracks

### Classical ML

The thesis describes Logistic Regression, SVM, Random Forest, KNN, and SGD experiments, plus an RSL ensemble of Random Forest, SVM, and Logistic Regression.

### Deep learning

The supplied notebooks implement 1D CNNs for tabular data. The final binary CNN notebook includes imputation, encoding, scaling, stratified splitting, class weighting, early stopping/checkpointing, and evaluation.

### Hybrid CNN + KNN

The conference paper and supplied notebooks use CNN feature extraction followed by KNN classification as the hybrid direction.

## Interpretation

The phrase "multi-modal" appears in the academic project title, but the supplied code and dataset are primarily tabular clinical data. The repository therefore uses the original title while making the implementation scope explicit.
