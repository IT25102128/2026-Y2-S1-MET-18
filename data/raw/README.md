# Raw Data

The assigned dataset is the **Credit Risk Dataset** from Kaggle:
https://www.kaggle.com/datasets/laotse/credit-risk-dataset

It is **not stored directly in this folder** because every notebook in this project
downloads it automatically at runtime with:

```python
import kagglehub
path = kagglehub.dataset_download("laotse/credit-risk-dataset")
```

To obtain a local copy of `credit_risk_dataset.csv` for manual inspection, either:

1. Run the first cell of `group_pipeline.ipynb` (requires a Kaggle account / API access), or
2. Download it directly from the Kaggle dataset page linked above and place
   `credit_risk_dataset.csv` in this folder.
