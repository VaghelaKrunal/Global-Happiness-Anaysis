# Global Happiness Analysis

**Repository:** Global-Happiness-Anaysis

## Overview

This repository contains a Jupyter notebook `Global Happiness.ipynb` that performs an exploratory data analysis (EDA) on global happiness datasets (2015–2018). The notebook loads CSV files, cleans data, visualizes trends, and compares country-level happiness metrics across years.

## Contents

* `Global Happiness.ipynb` — Main analysis notebook.
* `data/` (recommended) — Place CSV files here (e.g., `2015.csv`, `2016.csv`, `2017.csv`, `2018.csv`).

## Key Features

* Data cleaning and null-value handling
* Comparative bar plots and KDE plots of happiness scores
* Country-level ranking and top-k comparisons
* Correlation analysis between happiness score and its contributing factors

## Requirements

* Python 3.8+
* Jupyter Notebook / JupyterLab
* Packages:

  * pandas
  * numpy
  * matplotlib
  * seaborn

Install dependencies (recommended in a virtual environment):

```bash
python -m venv venv
source venv/bin/activate   # macOS / Linux
venv\Scripts\activate    # Windows
pip install --upgrade pip
pip install pandas numpy matplotlib seaborn jupyter
```

## How to run

1. Clone the repository:

```bash
git clone https://github.com/VaghelaKrunal/Global-Happiness-Anaysis.git
cd Global-Happiness-Anaysis
```

2. Ensure CSV files are in a `data/` folder or update paths in the notebook.
3. Launch Jupyter:

```bash
jupyter notebook
```

4. Open and run `Global Happiness.ipynb` step-by-step. Cells include comments and visualization outputs.

## Notebook notes & tips

* The notebook assumes CSV files use standard column names like `Country` and `Happiness Score`. If your CSV uses different headers, update the `read_csv` calls accordingly.
* If you run into parsing issues (e.g., separators), try `pd.read_csv('file.csv', sep=';')` or inspect the file encoding.
* The visualizations are built with `matplotlib` and `seaborn`; if plots don't render inline, ensure `%matplotlib inline` (for classic notebook) or use JupyterLab's plot viewer.

## Suggested Improvements

* Add a `requirements.txt` or `environment.yml` for reproducible environments.
* Move raw CSVs to a `data/` directory and add a small sample `data/.gitkeep` or sample CSVs.
* Add automated unit tests for data-cleaning functions.
* Create a script `run_analysis.py` to export static plots and summaries.

## License

Add a licen
