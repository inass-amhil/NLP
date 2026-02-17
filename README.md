# Multilingual Language Detection (English vs French)

## Project Overview

This project implements a **language detection system** that classifies sentences as either **English** or **French** using:

- Word2Vec embeddings
- Sentence vector averaging
- Logistic Regression classifier

The model achieves approximately **98% accuracy** on the test set.

## Dataset
## Dataset

The dataset used in this project was obtained from **Tatoeba**:

https://tatoeba.org

Tatoeba is a large collaborative database of sentences and translations in multiple languages.

### Dataset Description

- Total number of sentence pairs: **429,372**
- Each row contains:
  - `en` → English sentence
  - `fr` → Corresponding French translation

The dataset consists of parallel English–French sentences, meaning that each English sentence has its exact French equivalent.
From the 429,372 sentence pairs:

- English sentences were labeled as `0`
- French sentences were labeled as `1`
- Both were merged into a single dataset for binary classification

Note: The dataset is too large to be hosted directly on GitHub.

Please download it from:
https://drive.google.com/file/d/1eHMgsOe1Y6cRiYc3aInfnpOwPbfCKdpM/view?usp=drive_link

## Technologies Used

- Python 3
- Pandas
- NumPy
- Gensim (Word2Vec, FastText)
- Scikit-learn
- Google Colab

  
If running locally, install required libraries:

```bash
pip install gensim fasttext scikit-learn nltk
