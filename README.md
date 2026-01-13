# forskningsmetodik_2025_Delta2.0

This repository contains the code and notebooks used to evaluate the **DeLTA 2.0 single-cell analysis pipeline** for growth-based phenotypic drug susceptibility testing (pDST) on microfluidic time-lapse microscopy data. The analysis focuses on extracting population-level growth trends from segmented and tracked cells and comparing drug-treated versus control conditions.

## Project Overview

The work supports the accompanying course report “Evaluating DeLTA 2.0 for Growth-Based Drug Susceptibility Analysis in Microfluidic Time-Lapse Microscopy.” It includes:

- Growth-rate extraction and visualization (area and length)
- Temporal binning and smoothing
- Visualization and comparison of control vs drug conditions
- Calculation of percent change in area under the growth curve (AUC)

## Repository Contents
├── Example_analysis.ipynb # Example workflow on sample data
├── Analyzing_past_runs.ipynb # Analysis of previously processed results
├── training_plot.png # Visualization of segmentation model training
├── area-based_gr_trends.png # Example area growth curves
├── length-based_gr_trends.png # Example length growth curves
├── splitted_mask_overlay*.png # Examples of mask refinement results
├── paper.pdf # The paper via you found this paper
└── README.md # This file

## Getting Started

### Prerequisites

To run the analysis notebooks, you will need:

- Python 3.x
- Google Colab or Jupyter Notebook
- Standard scientific libraries: `numpy`, `pandas`, `matplotlib`
- `DeLTA 2.0` repository (as described in the report)

### Download Model Weights

The retrained model weights are hosted externally (e.g., Google Drive). Use the following snippet in Colab to download:

```bash
!pip install -q gdown
!gdown https://drive.google.com/uc?id=1CILkZPZuq8MO38Vp9qfIwFi99uiCdHyy
