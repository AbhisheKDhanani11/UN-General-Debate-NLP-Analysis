# NLP Exploration of United Nations Discourse: Trends in Topics and Language Patterns from General Debate Speeches

[![Paper Status](https://img.shields.io/badge/Status-Accepted-green)](https://bai26.org/) [![Python Version](https://img.shields.io/badge/Python-3.12-blue)](https://www.python.org/) [![License](https://img.shields.io/badge/License-MIT-yellow)](LICENSE)

This repository contains the code, notebook, figures, and accepted paper for our research on analyzing UN General Debate speeches using Natural Language Processing (NLP) techniques. The study covers over 4,700 speeches from 2000-2024, identifying trends in topics like climate change, security, and development via topic modeling (LDA/NMF) and visualizations.

The paper has been accepted to the 2026 International Conference on Breakthroughs in Artificial Intelligence (BAI’26), May 4-6, 2026, Sheraton Tunis Hotel, Tunis, Tunisia. It will appear in the conference proceedings in the Springer Book Series: Lecture Notes in Networks and Systems (LNNS). Publication is pending final camera-ready submission and presentation.

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


## Usage
- Open and run the Jupyter notebook: `UN_speech_notebook.ipynb` (use Jupyter Lab or VS Code).  
- It loads the data, performs preprocessing, topic modeling (LDA/NMF), sentiment analysis, and generates visualizations (e.g., heatmaps of keyword trends, pyLDAvis interactive topics).  
- Key sections: Data loading, preprocessing, visualizations, topic modeling.  
- To reproduce results: Ensure the dataset is in place and run cells sequentially. Outputs include figures in `/figures/` (exported manually if needed).

## Results
Key visualizations from the notebook (see full details in the paper). The figures highlighted below are those featured in the accepted paper:

- **Top Words 2000-2004** (Bar chart showing frequency of words like "international", "security", etc.)  
![Top Words 2000-2004](Figures/top_words_2000-2004.png)

- **Top Words 2005-2009** (Bar chart)  
![Top Words 2005-2009](Figures/top_words_2005-2009.png)

- **Top Words 2010-2014** (Bar chart)  
![Top Words 2010-2014](Figures/top_words_2010-2014.png)

- **Top Words 2015-2019** (Bar chart)  
![Top Words 2015-2019](Figures/top_words_2015-2019.png)

- **Top Words 2020-2024** (Bar chart)  
![Top Words 2020-2024](Figures/top_words_2020-2024.png)

- **Heatmap Economic** (Heatmap of Trade and Economic Words Across Years (2000-2024))  
![Heatmap Economic](Figures/heatmap_economic.png)

- **Heatmap Words Year** (Heatmap of Top Word Frequencies Across Years (2000-2024))  
![Heatmap Words Year](Figures/heatmap_words_year.png)

- **Heatmap Geopolitical** (Heatmap of Geopolitically Important Countries Across Years (2000-2024))  
![Heatmap Geopolitical](Figures/heatmap_geopolitical.png)

- **Heatmap Security** (Heatmap of Security and Terrorism Words Across Years (2000-2024))  
![Heatmap Security](Figures/heatmap_security.png)

- **Speech Length Period** (Average Speech Length by Five-Year Period)  
![Speech Length Period](Figures/speech_length_period.png)

- **Topic Proportions Over Time** (Stacked area chart from LDA)  
![Topic Proportions Over Time](Figures/topic_proportions_over_time.png)

- **Heatmap Words Decade** (Heatmap of Top 5 Word Frequencies Across Decades)  
![Heatmap Words Decade](Figures/heatmap_words_decade.png)

- **Word Trends Decade** (Word Frequency Trends by Decade)  
![Word Trends Decade](Figures/word_trends_decade.png)

- **Word Trends Period** (Word Frequency Trends by Five-Year Period)  
![Word Trends Period](Figures/word_trends_period.png)

- **TFIDF Heatmap Top Words Groups** (TF-IDF Scores of Top 20 Distinctive Words Across Groups)  
![TFIDF Heatmap Top Words Groups](Figures/tfidf_heatmap_top_words_groups.png)  
![TFIDF Heatmap Top Words Groups 1](Figures/tfidf_heatmap_top_words_groups1.png)

- **LDA Topic Proportions G7 G20 EU Africa** (Average LDA Topic Proportions Across Groups)  
![LDA Topic Proportions G7 G20 EU Africa](Figures/lda_topic_proportions_g7_g20_eu_africa.png)  
![LDA Topic Proportions G7 G20 EU Africa 1](Figures/lda_topic_proportions_g7_g20_eu_africa1.png)

- **Top GPE Mentions By Group** (Top 10 Geopolitical Entities (GPE) Mentioned by Group)  
![Top GPE Mentions By Group](Figures/top_gpe_mentions_by_group.png)  
![Top GPE Mentions By Group 1](Figures/top_gpe_mentions_by_group1.png)

- **Word Clouds** (Various thematic word clouds)  
Examples:  
![Topic0](Figures/topic0.png)  
![Topic1](Figures/topic1.png)  
![Topic2](Figures/topic2.png)  
![Topic3](Figures/topic3.png)  
![Topic4](Figures/topic4.png)  
![Topic5](Figures/topic5.png)  
![Topic6](Figures/topic6.png)  
![Topic7](Figures/topic7.png)  
![Topic8](Figures/topic8.png)  
![Topic9](Figures/topic9.png)

All figures are in the `/Figures/` folder. Those directly from the paper are prioritized above.
## Citation
If using this code or data, please cite the paper (once published):  
@article{dhanani2026nlp,
title={NLP Exploration of United Nations Discourse: Trends in Topics and Language Patterns from General Debate Speeches},
author={Dhanani, Abhishek and Patel, Jaymit and Senbel, Samah},
booktitle={2026 International Conference on Breakthroughs in Artificial Intelligence (BAI’26)},
year={2026},
publisher={Springer Lecture Notes in Networks and Systems (LNNS)},
url={https://github.com/AbhisheKDhanani11/UN-General-Debate-NLP-Analysis}
}

## Contact
For questions, reach out to dhanania@mail.sacredheart.edu or open an issue on GitHub.
