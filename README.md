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

- **Top 10 Words in 2000-2004** (Bar chart showing frequency of words like "international", "security", etc.)  
![Top 10 Words in 2000-2004](figures/top_words_2000-2004.png)

- **Top 10 Words in 2005-2009** (Bar chart)  
![Top 10 Words in 2005-2009](figures/top_words_2005-2009.png)

- **Top 10 Words in 2010-2014** (Bar chart)  
![Top 10 Words in 2010-2014](figures/top_words_2010-2014.png)

- **Top 10 Words in 2015-2019** (Bar chart)  
![Top 10 Words in 2015-2019](figures/top_words_2015-2019.png)

- **Top 10 Words in 2020-2024** (Bar chart)  
![Top 10 Words in 2020-2024](figures/top_words_2020-2024.png)

- **Heatmap of Trade and Economic Words Across Years (2000-2024)** (Highlighted in paper for economic trends)  
![Heatmap of Trade and Economic Words](figures/heatmap_economic.png)

- **Heatmap of Top Word Frequencies Across Years (2000-2024)** (Highlighted for overall trends)  
![Heatmap of Top Words](figures/heatmap_words_year.png)

- **Heatmap of Geopolitically Important Countries Across Years (2000-2024)** (Highlighted for regional focus)  
![Heatmap of Geopolitical Countries](figures/heatmap_geopolitical.png)

- **Heatmap of Security and Terrorism Words Across Years (2000-2024)**  
![Heatmap of Security and Terrorism](figures/heatmap_security.png)

- **Average Speech Length by Five-Year Period** (Line chart showing speech length trends)  
![Average Speech Length](figures/speech_length_period.png)

- **Topic Proportions Over Time** (Stacked area chart from LDA)  
![Topic Proportions Over Time](figures/topic_proportions_over_time.png)

- **Heatmap of Top 5 Word Frequencies Across Decades**  
![Heatmap Top 5 Words Decades](figures/heatmap_words_decade.png)

- **Word Frequency Trends by Decade** (Line chart)  
![Word Frequency Trends Decade](figures/word_trends_decade.png)

- **Word Frequency Trends by Five-Year Period** (Line chart)  
![Word Frequency Trends Five-Year](figures/word_trends_period.png)

- **TF-IDF Scores of Top 20 Distinctive Words Across Groups** (Heatmaps for G7, G20, EU, Africa)  
![TF-IDF Heatmap 1](figures/tfidf_heatmap_top_words_groups.png)  
![TF-IDF Heatmap 2](figures/tfidf_heatmap_top_words_groups1.png)

- **Average LDA Topic Proportions Across Groups** (Bar charts for topic distributions)  
![LDA Proportions 1](figures/lda_topic_proportions_g7_g20_eu_africa.png)  
![LDA Proportions 2](figures/lda_topic_proportions_g7_g20_eu_africa1.png)

- **Top 10 Geopolitical Entities (GPE) Mentioned by Group** (Bar charts for G7, G20, EU, Africa)  
![Top 10 GPE by Group 1](figures/top_gpe_mentions_by_group.png)  
![Top 10 GPE by Group 2](figures/top_gpe_mentions_by_group1.png)

- **Word Clouds** (Various thematic word clouds)  
Examples:  
![Word Cloud Topic 0](figures/topic0.png)  
![Word Cloud Topic 1](figures/topic1.png)  
![Word Cloud Topic 2](figures/topic2.png)  
![Word Cloud Topic 3](figures/topic3.png)  
![Word Cloud Topic 4](figures/topic4.png)  
![Word Cloud Topic 5](figures/topic5.png)  
![Word Cloud Topic 6](figures/topic6.png)  
![Word Cloud Topic 7](figures/topic7.png)  
![Word Cloud Topic 8](figures/topic8.png)  
![Word Cloud Topic 9](figures/topic9.png)

All figures are in the `/figures/` folder. Those directly from the paper are prioritized above.

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
