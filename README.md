# CUES-Surv: Dynamic Evaluation of Survival Models

[![Python Version](https://img.shields.io/badge/python-3.8%2B-blue)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![DOI](https://img.shields.io/badge/DOI-10.5281/zenodo.XXXXXX-blue)](https://doi.org/10.5281/zenodo.XXXXXX)

**CUES-Surv** is a comprehensive evaluation framework for survival analysis models. It computes a dynamic composite score that integrates **Calibration**, **Utility**, **Equity**, and **Stability** over time, while also reporting standard metrics like the **C-index** and **Integrated Brier Score (IBS)**.

This repository contains the Python implementation used in our paper:  
> Ali Mohammad Alqudah, and Zahra Moussavi. "CUES: A Multiplicative Composite Metric for Evaluating Clinical Prediction Models Theory, Inference, and Properties." Mathematics 14.3 (2026): 398. [https://doi.org/10.3390/math14030398](https://doi.org/10.3390/math14030398)

## Features
- Supports **7 public datasets** (GBSG2, WHAS500, AIDS, CGVHD, Breast Cancer, FLCHAIN, Veterans Lung Cancer) – BMT has been removed for clarity.
- Models: **Penalized CoxPH**, **Random Survival Forest**, **Gradient Boosting Survival**.
- Handles **missing values** via median/most_frequent imputation.
- Uses **IPCW** (Inverse Probability of Censoring Weighting) for unbiased Brier score and utility.
- Computes **CUES‑Surv** scores dynamically over any user-defined time horizon.
- Produces **trajectory plots**, **component plots**, and **actual vs. predicted survival curves**.
- Reports **Concordance Index** (C‑index) and **Integrated Brier Score** alongside CUES components.

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/cues-surv.git
cd cues-surv
