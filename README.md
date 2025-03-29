## Summary of Methods

* **Ligand pose**: Templated docking (FlexX) using the complex in training set with the maximum MCS similarity i.e. N(1) closest neighbor as template. The pose with the best Hyde score and without unfavorable torsion is selected.
* **Potency/ADMET**: Ensemble of tree-based algorithm (Random forest, LightGBM, XGBoost, ExtraTrees), chemprop, and TabPFN trained on ECFP4 + physchem + extra features (derived from external public dataset). This approach is similar to our recent [publication in ACS Medicinal Chemistry Letters](https://pubs.acs.org/doi/10.1021/acsmedchemlett.4c00505 )  Note: No hyperparameter optimization was performed.
