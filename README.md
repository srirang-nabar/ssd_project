
Project: Statistical Structures in Data — Sunspots & Daylight Analysis
=============================================================

This repository contains exploratory data analysis and a small non-parametric regression study prepared as part of a college assignment for the course "Statistical Structures in Data" (PGDBA, Semester 1).

**Purpose:**
- **Analyze sunspot activity** through time and demonstrate kernel regression smoothing on monthly sunspot counts.
- **Explore daylight/sunrise–sunset data** (daylength) and supporting visualizations.

Files Overview
--------------
- **`EDA_sunspots.ipynb`**: Exploratory data analysis for the processed sunspot dataset. Loads `sunspot_data_processed.csv`, cleans a few columns, and plots monthly mean sunspot numbers over time.
- **`kernel_regression.ipynb`**: Fits a kernel regression (using `statsmodels.nonparametric.kernel_regression.KernelReg`) to the sunspot data, inspects bandwidths, R^2, and visualizes the fitted curves for multiple bandwidth values.
- **`sunspot_data_processed.csv`**, : Data file used by the notebooks and scripts.

Getting Started
---------------
Recommended environment (project includes a `pyproject.toml` with dependencies):

1. Create a virtual environment and activate it:

```
python3.13 -m venv .venv
source .venv/bin/activate
```

2. Install the project dependencies from `pyproject.toml` (PEP 621):

```
pip install .
```

Or install dependencies manually with pip, for example:

```
pip install numpy pandas matplotlib statsmodels notebook
```

Notes & Tips
------------
- The notebooks assume the CSV data files are in the repository root. If you move data files, update the paths at the top of the notebooks.
- The `kernel_regression.ipynb` uses `statsmodels`'s `KernelReg`. If you encounter performance or version issues, please ensure `statsmodels>=0.14.5` (see `pyproject.toml`).

Acknowledgements
----------------
The dataset we used comes from the following dataset:
 - [Kaggle Dataset: Monthly Mean Sunspot Numbers from 1749 to Present](https://www.kaggle.com/datasets/hamtaghanbaripour/monthly-mean-sunspot-numbers-from-1749-to-present/data)

Contact / Author
----------------
- Author: Srirang Nabar
- Course: PGDBA — Statistical Structures in Data (Semester 1)
