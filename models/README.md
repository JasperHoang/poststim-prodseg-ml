# Trained model release

This directory contains the 12 GridSearchCV-selected model pipelines used in the EAGE 2025 workflow.

## Naming convention

Each file follows `best_model_<pipeline>.joblib`:

- `PS`: StandardScaler + PCA
- `PFS`: StandardScaler + PolynomialFeatures
- `PR`: RobustScaler + PCA
- `PFR`: RobustScaler + PolynomialFeatures
- `XGB`: XGBoost regressor
- `RF`: Random Forest regressor
- `NN`: MLP neural-network regressor

The reported best pipeline is `best_model_pfs-nn.joblib`.

## Contents

- `trained/`: 12 serialized scikit-learn-compatible model pipelines
- `metadata/`: model explanations and well-level notes from the training workflow
- `figures/`: SVG model-comparison figures

Load serialized models only in a trusted Python environment with compatible dependency versions. Joblib files can execute arbitrary code during deserialization and should never be loaded from untrusted sources.
