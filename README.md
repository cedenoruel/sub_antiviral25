## Summary of Methods

* **Ligand pose**: Templated docking (FlexX) using the complex in training set with the maximum MCS similarity. The pose with the best Hyde score and without unfavorable torsion is selected.
* **Potency/ADMET**: Ensemble of tree-based algorithm (Random forest, LightGBM, XGBoost, ExtraTrees) trained on ECFP4 + physchem + extra features (derived from external public dataset). 
