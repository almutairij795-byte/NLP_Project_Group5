# Sentiment Analysis: The Effect of Word Bigrams on Negation

## Project Overview
This project investigates whether adding word bigram features improves sentiment classification, particularly for reviews containing negation.

We compare three classification models:
1. TF-IDF Unigram + Logistic Regression
2. TF-IDF Unigram + Bigram + Logistic Regression
3. Sentence-BERT (`all-MiniLM-L6-v2`) + Logistic Regression

## Dataset
We used the Sentiment Labelled Sentences dataset from the UCI Machine Learning Repository, containing reviews from three domains:
- Amazon
- IMDb
- Yelp

The dataset is downloaded automatically when the notebook is executed.

## Methodology
- Data cleaning and preprocessing.
- 70% training, 15% development, and 15% testing split.
- Hyperparameter tuning using the development set.
- Evaluation on the full test set and a negation subset.
- Performance measured using Accuracy and Macro F1.

## Repository Structure
- `Review_Sentiment_Negation_Notebook_Final.ipynb`: Main notebook containing the implementation and analysis.
- `results/`: CSV files containing cleaning audits, model results, data splits, and error analysis.
- `figures/`: Figures generated during the experiments.

## How to Run
1. Open the notebook using Google Colab.
2. Run all cells in order.
3. Allow the notebook to download the dataset and required models or libraries.
4. Review the generated results and figures.

## Models and Tools
- Python
- Google Colab
- Scikit-learn
- Sentence-Transformers
- Pandas
- NumPy
- Matplotlib

## Evaluation
All three models were evaluated using the same held-out test set. We also evaluated their performance on the negation subset to examine how they handle negation in sentiment classification.

## Authors
Group project – Artificial Intelligence Program.
