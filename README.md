# CUES-Surv: Dynamic Evaluation of Survival Models

This repository contains the Python implementation of **CUES-Surv**, a comprehensive evaluation framework for survival analysis models. It computes a dynamic composite score combining **Calibration**, **Utility**, **Equity**, and **Stability** over time.

## Features
- Evaluates **Penalized CoxPH**, **Random Survival Forest**, and **Gradient Boosting Survival** models.
- Supports **7 public datasets** (GBSG2, WHAS500, AIDS, BMT, CGVHD, Breast Cancer, FLCHAIN, Veterans Lung Cancer).
- Handles **missing values** via imputation.
- Uses **IPCW** (Inverse Probability of Censoring Weighting) for unbiased Brier score and net benefit.
- Produces **trajectory plots**, **component plots**, and **summary tables**.
- Outputs a **CUES‑Surv score** that integrates four key aspects of model performance.

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/cues-surv.git
cd cues-surv
