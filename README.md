# Real Estate Price Prediction

Project repository for predicting property prices using a dataset of real estate listings and an interactive analysis notebook.

## Contents
- **Dataset:** [Final_property_data.csv](Final_property_data.csv) — cleaned dataset used for training and evaluation.
- **Notebook:** [price_prediction.ipynb](price_prediction.ipynb) — exploratory data analysis, preprocessing, feature engineering, model training, and evaluation.
- **Metadata:** [property_meta.json](property_meta.json) — metadata for property fields.
- **Property-level data:** [property_level.json](property_level.json) — additional structured property data.
- **Unseen samples:** [property_unseen.json](property_unseen.json) — example/unseen properties for running predictions.

## Overview
This project demonstrates a workflow to predict real estate property prices using Python. The analysis is contained in the Jupyter notebook `price_prediction.ipynb`, which walks through data loading, cleaning, feature engineering, model training, and basic evaluation.

## Requirements
- Python 3.9+ (recommended)
- Common libraries: `pandas`, `numpy`, `scikit-learn`, `xgboost`, `matplotlib`, `seaborn`, `jupyter`

You can install the common dependencies with:

```bash
python -m venv venv
venv\Scripts\activate     
pip install --upgrade pip
pip install pandas numpy scikit-learn xgboost matplotlib seaborn jupyter
```

If you prefer a `requirements.txt`, create one from your environment after installing packages:

```bash
pip freeze > requirements.txt
```

## Running the analysis
1. Ensure `Final_property_data.csv` is in the repository root (or update file paths in the notebook).
2. Start Jupyter Lab/Notebook:

```bash
jupyter notebook
# or
jupyter lab
```

3. Open [price_prediction.ipynb](price_prediction.ipynb) and run cells sequentially. Adjust file paths or parameters as needed.

## Reproducing model training and predictions
- Use the notebook to reproduce preprocessing and model training steps.
- To generate predictions for new/unseen properties, load `property_unseen.json`, apply the same preprocessing pipeline, then call the trained model's `predict` method. The notebook includes example code snippets for this flow.

## Notes & Tips
- If long-running model training is included, consider saving trained models to disk using `joblib` or `pickle` for reuse.
- For larger experiments, extract core training and inference code into standalone scripts (e.g., `train.py`, `predict.py`).

## License & Contact
This repository does not include an explicit license. If you want to share it, consider adding an open-source license file.

- **Author:** Mohammed Shoeb
- **Repository:** https://github.com/shoaibms27/-Real-Estate-Price-Prediction

For questions or help, open an issue in the repository or contact the author.
