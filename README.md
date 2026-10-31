# Alzheimer's Disease Prediction Using Handwriting, Clinical Data and AI Models

This project predicts Alzheimer's disease from three kinds of data: handwriting dynamics, clinical and MRI-derived measures, and brain MRI images. It compares classical machine learning with CNNs and explains the predictions with LIME.

## Data

| Data | Source | File |
| --- | --- | --- |
| Handwriting features for 174 participants (pen pressure, speed, in-air time and similar, over 25 tasks) | [DARWIN dataset, UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/732/darwin) | `data.zip` (`data.csv`) |
| Longitudinal clinical and MRI-derived measures (MMSE, CDR, eTIV, nWBV, ASF) | [OASIS-2](https://sites.wustl.edu/oasisbrains/) | `Alzheimer clinical data.csv` |
| Brain MRI slices in 4 dementia classes | [Kaggle: Alzheimer's Dataset (4 classes)](https://www.kaggle.com/datasets/tourist55/alzheimers-dataset-4-class-of-images/), derived from OASIS | Not included |

See `Dataset documentation of Alzheimer 4D image data.pdf` for details.

## Notebooks

| Notebook | Purpose |
| --- | --- |
| `Cognitive_ done by sufi_30_11_2023.ipynb` | Handwriting-based prediction with tree ensembles and Naive Bayes |
| `Explainable__LIME_Alzheimer_disease_prediction_analysis.ipynb` | Random forest on handwriting features with LIME explanations |
| `alzheimer_clinical_validation_code_22_04_2024.ipynb` | Clinical validation on OASIS-2: exploratory analysis, imputation, then logistic regression, SVM, decision tree, random forest and AdaBoost |
| `alzheimer_disease_prediction_by__CNN_Model.ipynb` | CNN classifier on MRI slices (TensorFlow) |
| `Alzheimer_additional_analysis*.ipynb` | MRI segmentation, affected-region visualisation and annotation |
| `Combined_Figure_Alzheimer.ipynb` | Combined figure for the write-up |

## Running it

```bash
pip install pandas numpy scikit-learn tensorflow lime matplotlib seaborn plotly scikit-image opencv-python
```

The notebooks were written in Google Colab and read from `/content/`. Change these paths to run them locally.

## Licence

No licence has been declared yet. DARWIN is released under CC BY 4.0. OASIS data are subject to the [OASIS data use terms](https://sites.wustl.edu/oasisbrains/).

## Author

Md Abu Sufian - ORCID [0009-0007-3503-6942](https://orcid.org/0009-0007-3503-6942)
