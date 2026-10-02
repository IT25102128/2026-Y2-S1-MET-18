# IT2011 - Artificial Intelligence and Machine Learning

## Group Project

### Group ID
2026-Y2-S1-MET-18

### Project Overview
This project implements an end-to-end data preprocessing pipeline on the Credit Risk Dataset. The workflow covers duplicate handling, missing value imputation, outlier detection, categorical encoding, feature selection, and standardization to prepare the data for machine learning modeling.

### Dataset
- **Assigned Dataset:** Credit Risk Dataset
- **Source:** Kaggle (`laotse/credit-risk-dataset`)
- **Target Variable:** `loan_status` (0 = non-default, 1 = default)
- **Access Method:** Downloaded at runtime via `kagglehub.dataset_download("laotse/credit-risk-dataset")`

### Project Structure
- `data/raw/` — original assigned dataset
- `data/processed/` — cleaned/preprocessed datasets
- `data/external/` — external datasets if used
- `notebooks/preprocessing/` — individual preprocessing contributions
- `notebooks/models/` — individual machine learning models
- `group_pipeline.ipynb` — integrated group pipeline
- `results/eda_visualizations/` — EDA graphs
- `results/model_results/` — individual model evaluation results
- `results/model_comparison/` — final comparison of the six models
- `results/outputs/` — generated datasets/features/output files
- `results/logs/` — execution logs if required
- `team_contributions/` — reserved for later contribution documentation
- `documentation/` — proposal, progress review material, report and presentation

### Preprocessing Contributions

| IT Number | Preprocessing Technique |
|-----------|-------------------------|
| IT25102121 | Standardization / Scaling |
| IT25102122 | Handling Missing Data |
| IT25102123 | Feature Selection |
| IT25102124 | Outlier Detection |
| IT25102128 | Duplicate Data Handling |
| IT25102129 | One-Hot Encoding |

### Running the Project
1. Install project dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn kagglehub
   ```
2. Open and run `group_pipeline.ipynb` in Jupyter Notebook / JupyterLab or Google Colab from top to bottom. The dataset is fetched automatically via `kagglehub`.
3. Alternatively, individual preprocessing contributions can be run independently from `notebooks/preprocessing/`.
4. Outputs and generated processed data will be saved to `results/outputs/`.