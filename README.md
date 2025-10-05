# DA5401 Assignment 5: Visualizing Data Veracity Challenges in Multi-Label Classification

## Overview

This assignment explores the Yeast gene expression dataset using advanced dimensionality reduction techniques (t-SNE and Isomap) to visually inspect data veracity issues such as noisy labels, outliers, and hard-to-learn samples in a multi-label classification context.

## Files

- `assignment_5.ipynb` — Main Jupyter Notebook with all code, visualizations, and analysis.
- `yeast.arff` — Yeast dataset in ARFF format (features + multi-labels).
- `yeast.xml` — Label definitions for the Yeast dataset.

## Requirements

- Python 3.7+
- Jupyter Notebook
- Required packages:
  - numpy
  - matplotlib
  - scikit-learn
  - liac-arff

Install dependencies with:
```bash
pip install numpy matplotlib scikit-learn liac-arff
```

## How to Run

1. Place all files (`assignment_5.ipynb`, `yeast.arff`, `yeast.xml`) in the same directory.
2. Open `assignment_5.ipynb` in Jupyter Notebook or VS Code.
3. Run all cells in order to reproduce the analysis and visualizations.

## Assignment Structure

- **Data Loading:** Loads the ARFF file and extracts features and multi-label targets.
- **Dimensionality Check:** Reports the shape of the feature and label matrices.
- **Label Selection for Visualization:** Simplifies the 14-label problem to 4 categories for clear plotting.
- **Scaling:** Standardizes features for fair distance-based analysis.
- **t-SNE & Isomap:** Applies both techniques, visualizes results, and inspects for data veracity issues.
- **Analysis & Discussion:** Answers conceptual questions and discusses findings.

## Results Summary

- **t-SNE** reveals local clusters and highlights ambiguous labels, outliers, and mixed regions.
- **Isomap** preserves global structure, showing the overall manifold and cluster relationships.
- **Conclusion:** Both methods provide complementary insights into the challenges of multi-label biological data.

## Notes

- If you encounter errors about missing single-label classes, the notebook handles these cases gracefully.
- The notebook is fully commented for clarity and reproducibility.

