# BBC News Analysis — NER & Text Classification

Named Entity Recognition and category classification on 42,115 BBC News articles using spaCy and Logistic Regression.

## Overview
This project extracts named entities from BBC News articles, analyses which people, organisations and locations dominate the news, and builds a classifier to predict article category from description text.

## What's covered
- Named Entity Recognition with spaCy — extracting PERSON, ORG, GPE, NORP, EVENT entities
- Entity frequency analysis — most mentioned people, organisations and locations
- Category extraction from URLs (UK, World, Sport, Business-Tech, Entertainment, Health-Education)
- Logistic Regression classifier with TF-IDF + bigrams — 75% accuracy across 6 categories
- Entity-based classification experiment — testing entities as features vs full text (23% vs 75%)
- Visualisations: entity bar charts

## Dataset
[BBC News Archive](https://www.kaggle.com) via Kaggle — 42,115 articles covering news from 2022.

## Key findings
- Sport was the easiest category to classify (95% precision) — highly distinctive vocabulary
- Ukraine and Russia appear 983 and 700 times — dataset captures the early 2022 invasion
- Using NER entities alone as features dropped accuracy from 75% to 23% — context words matter as much as named entities

## Libraries
- pandas, numpy
- spacy
- scikit-learn
- matplotlib

## Author
GreenBlueberryKate
