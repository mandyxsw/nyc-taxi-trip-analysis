# NYC Taxi Trip Analysis

An end-to-end NYC HVFHV trip analysis project covering data retrieval and wrangling, EDA, baseline supervised modeling, unsupervised learning, feature engineering, and advanced supervised learning.

## Overview

This project analyzes trip-level data from the NYC Taxi and Limousine Commission (TLC) High Volume For-Hire Vehicles (HVFHV) dataset.

The project includes:

- data retrieval and wrangling,
- exploratory data analysis (EDA),
- baseline supervised modeling,
- unsupervised learning and feature engineering,
- advanced supervised learning,
- final report and executive summary,
- a lightweight machine learning results dashboard.

## Repository Structure

```text
Notebooks/
├── Phase_1_Data_Retrieval_and_Wrangling.ipynb
├── Phase_1_EDA_and_Baseline_Modeling.ipynb
├── Phase_2_Supervised_Learning_and_Feature_Engineering.ipynb
├── Phase_2_Unsupervised_Learning_and_Feature_Engineering.ipynb
├── Phase_3_Data_Retrieval_and_Wrangling.ipynb
├── Phase_3_EDA_&_Baseline_Modeling.ipynb
├── Phase_3_ML_Results_Dashboard.ipynb
├── Phase_3_Supervised_Learning.ipynb
└── Phase_3_Unsupervised_Learning.ipynb

Reports/
├── Division_of_Labor.txt
├── Ethical Considerations.pdf
├── Executive_Summary.pdf
├── Final_Report.pdf
├── Phase_2_Supervised_Learning_and_Feature_Engineering.pdf
├── Phase_2_Unsupervised_Learning_and_Feature_Engineering.pdf
├── Phase_3_Data_Retrieval_and_Wrangling.pdf
├── Phase_3_EDA_&_Baseline_Modeling.pdf
├── Phase_3_Supervised_Learning.pdf
└── Phase_3_Unsupervised_Learning.pdf
```

## Key Results

- `trip_miles` has a strong positive relationship with `driver_pay`.
- The baseline linear regression model provides a stable and interpretable benchmark.
- Unsupervised learning identifies meaningful trip behavior patterns.
- Advanced supervised models improve predictive performance over the baseline.
- Full-dataset validation supports the robustness of the clustering workflow.

## Requirements

This repository was developed primarily with Python notebooks. A minimal environment is provided in [`requirements.txt`](requirements.txt).

Recommended:

- Python 3.10+
- Jupyter Notebook or JupyterLab

Install dependencies with:

```bash
pip install -r requirements.txt
```

## Data

Large raw and processed datasets are not included in this repository.

To run the notebooks locally, place the cleaned parquet files in a location accessible from your environment. Several notebooks currently expect local or Google Drive based paths, so you may need to update the dataset path variables near the top of each notebook before running them.

Typical files referenced by the notebooks include:

- `tripdata_clean_full.parquet`
- `tripdata_clean_eda_5M.parquet`
- `tripdata_sample_100k.parquet`

## How to Run

1. Clone the repository.
2. Create and activate a Python environment.
3. Install dependencies with `pip install -r requirements.txt`.
4. Launch Jupyter Notebook or JupyterLab.
5. Open the notebook you want to run from the `Notebooks/` folder.
6. Update any dataset path variables if needed, then run the notebook cells in order.

Example:

```bash
git clone https://github.com/mandyxsw/nyc-taxi-trip-analysis.git
cd nyc-taxi-trip-analysis
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
jupyter notebook
```

## Suggested Reading Order

If you want a quick project walkthrough, this order works well:

1. `Phase_3_Data_Retrieval_and_Wrangling.ipynb`
2. `Phase_3_EDA_&_Baseline_Modeling.ipynb`
3. `Phase_3_Unsupervised_Learning.ipynb`
4. `Phase_3_Supervised_Learning.ipynb`
5. `Phase_3_ML_Results_Dashboard.ipynb`

## Notes

This repository focuses on the final notebooks, reports, and project deliverables rather than shipping the full raw dataset.