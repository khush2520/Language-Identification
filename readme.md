
Certainly! Here's the updated Readme for Jupyter notebooks:

---

## Language Identification using n-grams

This repository contains Jupyter notebooks for identifying languages between Spanish (spa), Portuguese (por), Polish (pol), and Czech (ces) using n-gram analysis.
This repo also contains the dataset used and csv files with the predictionsPrerequisites

- Jupyter Notebook
- Python 3.x
- Pandas library

### Notebooks Overview

#### Spanish-Portuguese Identification

- **Notebook:** `Language_Identification_Spa_Por.ipynb`
- **Functions:**
  - `ngrams(df, n)`: Generates n-gram counts for Spanish and Portuguese texts.
  - `classify(df, n, ngrams_spa, ngrams_por)`: Classifies data based on n-gram counts.
  - `classify_zero(df, n, ngrams_spa, ngrams_por)`: Classifies data, handling zero-count n-grams.
- **Outputs:**
  - JSON files: `spaish_{i}grams.json` and `czech_{i}grams.json`.
  - CSV files: Classified results using different n-gram sizes.
  - Precision and recall scores for each n-gram size.
- **Usage:**
  - Modify n-gram sizes for optimal performance.
  - Evaluate precision and recall scores for classification performance.

#### Polish-Czech Identification

- **Notebook:** `Language_Identification_Pol_Ces.ipynb`
- **Functions:**
  - `ngrams(df, n)`: Generates n-gram counts for Polish and Czech texts.
  - `classify(df, n, ngrams_pol, ngrams_ces)`: Classifies data based on n-gram counts.
  - `classify_zero(df, n, ngrams_pol, ngrams_ces)`: Classifies data, handling zero-count n-grams.
- **Outputs:**
  - JSON files: `polish_{i}grams.json` and `czech_{i}grams.json`.
  - CSV files: Classified results using different n-gram sizes.
  - Precision and recall scores for each n-gram size.
- **Usage:**
  - Modify n-gram sizes for optimal performance.
  - Evaluate precision and recall scores for classification performance.

### Evaluation

- Precision and recall scores help assess the accuracy of language identification.
- Handling zero-count n-grams impacts classification accuracy and is addressed in the notebooks.
- Adjust n-gram sizes based on the dataset and expected language patterns.

### References

- [Pandas Documentation](https://pandas.pydata.org/docs/)
- [Scikit-learn Precision and Recall Scores](https://scikit-learn.org/stable/modules/generated/sklearn.metrics.precision_score.html)
- [Jupyter Notebook Documentation](https://jupyter.org/documentation)
