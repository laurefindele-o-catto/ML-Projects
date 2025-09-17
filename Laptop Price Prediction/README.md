Project Overview:

This project builds and evaluates machine learning models to predict laptop prices based on their specifications (CPU, RAM, storage, display, brand, etc.).
The goal is twofold:
- Achieve strong predictive performance using modern ensemble methods.
- Provide interpretability through feature importance, permutation importance, and SHAP values.
The final model is a Voting Ensemble (CatBoost + XGBoost + ExtraTrees), which outperforms individual models and generalizes well.

Features:

- Data Preprocessing Pipeline
    - Custom transformers for skew handling, scaling, and categorical encoding.
    - Robust handling of outliers and rare categories.
- Models Implemented
    - CatBoost
    - XGBoost
    - ExtraTrees
    - Voting Ensemble
    - Stacking Ensemble
- Evaluation Metrics
    - MAE, RMSE, R², MAPE
    - Train vs Test comparison to check for overfitting
    - Interpretability
- Built‑in feature importance (tree models)
    - Permutation importance (model‑agnostic)
    - SHAP values (global + local explanations)
- Visualizations
    - Residual plots
    - Predicted vs True scatter plots
    - Error distribution histograms
    - Correlation heatmap
    - Feature importance bar charts
    - SHAP summary & dependence plots

Results:
- Best Single Model: XGBoost (R² ≈ 0.818)
- Best Overall Model: Voting Ensemble (R² ≈ 0.823, lowest RMSE)
- Models generalize well with no severe overfitting.
- Key drivers of price: RAM, CPU tier, SSD presence, display quality (PPI/Inches), and brand.

