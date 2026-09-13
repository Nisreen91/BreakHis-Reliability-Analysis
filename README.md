# BreakHis Reliability Analysis

This repository contains the analysis notebook accompanying the study on patient-level reliability and calibration in breast histopathology classification using the BreakHis dataset.

## Repository Contents

- `BreakHis_Final_Paper_Analysis.ipynb`: Recomputes the patient-level metrics and generates the manuscript tables and figures from saved prediction files.

## Analyses Included

- Patient-level classification evaluation
- Accuracy, balanced accuracy, macro-F1, sensitivity, and specificity
- AUROC and AUPRC
- Brier score, negative log-likelihood, and expected calibration error
- Bootstrap confidence intervals using 500 resamples
- Confusion matrices
- ROC and precision-recall curves
- Reliability diagrams
- Aggregation-strategy comparisons
- Cross-magnification probability analysis

The notebook does not train or fine-tune models.

## Requirements

- Python 3
- NumPy
- pandas
- Matplotlib
- scikit-learn
- Google Colab

## Data and Prediction Files

The BreakHis dataset is not included in this repository. The notebook requires the saved prediction and analysis files generated during the original experiments.

Place the required files in a `results` directory or change the `RESULTS_DIR` variable in the first notebook cell to their location.

The current configuration uses:

```python
RESULTS_DIR = "/content/drive/MyDrive/BreakHis_Project/results"
