# Text-Sentiment-Analysis


This repository contains code for performing sentiment analysis on the Sentiment140 dataset using the VADER (Valence Aware Dictionary and sEntiment Reasoner) sentiment analysis tool.

## Why This Project?

Sentiment analysis is a crucial aspect of understanding public opinion, brand perception, and customer satisfaction. With the rise of social media, analyzing sentiments expressed in tweets can provide valuable insights for businesses, researchers, and policymakers. This project aims to leverage the power of VADER, a popular sentiment analysis tool, to classify the sentiment of tweets from the Sentiment140 dataset.

The primary goals of this project are:
- **Educational Purpose**: To demonstrate the end-to-end process of sentiment analysis using a real-world dataset, from data acquisition and preprocessing to model evaluation.
- **Practical Application**: To create a user-friendly tool that can help businesses and individuals analyze the sentiment of textual data easily.
- **Exploration of Natural Language Processing (NLP)**: To explore NLP techniques such as tokenization, stemming, POS tagging, and chunking, and understand their impact on sentiment analysis.
## Dataset

The Sentiment140 dataset consists of 1.6 million tweets that have been annotated for sentiment. The sentiment labels are:
- `0` for negative sentiment
- `4` for positive sentiment (which is converted to `1` in this project)

## Requirements

- Python 3.x
- NLTK
- Pandas
- Scikit-learn
- Kaggle API


## Setup

1. **Install dependencies:**

    ```bash
    pip install numpy pandas nltk scikit-learn kaggle streamlit
    ```

2. **Download the NLTK data packages:**

    In the `sentiment_analysis.py` script, the necessary NLTK data packages are downloaded automatically using:

    ```python
    nltk.download('stopwords')
    nltk.download('punkt')
    nltk.download('averaged_perceptron_tagger')
    nltk.download('vader_lexicon')
    ```

3. **Kaggle API Setup:**

    To download the Sentiment140 dataset from Kaggle, you need to set up the Kaggle API. Create a `kaggle.json` file with your Kaggle API credentials and place it in the appropriate directory.

    ```bash
    mkdir -p ~/.kaggle
    cp kaggle.json ~/.kaggle/
    chmod 600 ~/.kaggle/kaggle.json
    ```

