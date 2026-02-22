# NLP Exploration of United Nations Discourse: Trends in Topics and Language Patterns from General Debate Speeches

[![Paper Status](https://img.shields.io/badge/Status-Accepted-green)](https://example.com/paper-link) [![Python Version](https://img.shields.io/badge/Python-3.12-blue)](https://www.python.org/) [![License](https://img.shields.io/badge/License-MIT-yellow)](LICENSE)

This repository contains the code, notebook, and paper for my accepted research on analyzing UN General Debate speeches using Natural Language Processing (NLP) techniques. The study covers over 4,700 speeches from 2000-2024, identifying trends in topics like climate change, security, and development via topic modeling (LDA/NMF) and visualizations.

## Abstract (from the Paper)
This study analyzes historical speeches from the United Nations General Debate, spanning multiple decades, to uncover trends in topics and language usage. Utilizing a dataset of over 4,700 speeches from various countries and years, we apply natural language processing (NLP) techniques in Python to process and visualize the data. Key methods include tokenization with NLTK and spaCy for text cleaning, word frequency counting for visualizations like word clouds and histograms, and topic modeling via Latent Dirichlet Allocation (LDA) and Non-Negative Matrix Factorization (NMF) to identify dominant topics such as international peace, economic development, and conflict resolution. The analysis reveals evolving patterns, including a shift toward climate and inequality discussions in recent years and regional variations in language focus. Visualizations highlight topic proportions over time, showing increasing emphasis on sustainability post-2000, as well as the different issues of interest for different countries.

**Authors**: Abhishek Dhanani, Jaymit Patel, and Samah Senbel  
**Institution**: Sacred Heart University  
**Keywords**: UN Speeches, Natural Language Processing, Topic Modeling, Data Visualization, Python, LDA, NMF  

[Full Paper (DOCX)](NLP_paper.docx) | [Full Paper (PDF)](NLP_paper.pdf)  

## Dataset
The dataset is sourced from the United Nations General Debate Corpus on [Harvard Dataverse](https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/0TJX8Y). It includes ~4,700 speeches (2000-2024).  
- Download and place `Speakers_with_speeches_cleaned1.xlsx` in the `/data/` folder (or use the provided link in the notebook).  
- Note: The dataset is not uploaded here due to size; fetch it from the source for reproduction.

## Installation and Dependencies
1. Clone this repository:  
