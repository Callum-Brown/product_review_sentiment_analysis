# Sentiment Analysis of Amazon Customer Reviews

## Overview

This project involves analyzing sentiment from customer reviews of Amazon products using Python and natural language processing (NLP) techniques. The project classifies reviews into positive or negative sentiments based on textual analysis.

## Data

The dataset consists of Amazon customer reviews obtained from:

* `Datafiniti_Amazon_Consumer_Reviews_of_Amazon_Products_May19.csv`

## Libraries and Tools

* **Python**
* **Pandas** for data manipulation
* **NLTK** for natural language processing

  * Tokenization
  * Stopword removal
  * Stemming (using SnowballStemmer)
  * Sentiment analysis (using SentimentIntensityAnalyzer)

## Methodology

### Preprocessing

* Text tokenization
* Removal of stop words (common non-contributive words)
* Stemming to normalize words to their root forms

### Sentiment Classification

* Reviews are labeled as positive (rating > 2) or negative (rating ≤ 2)
* Sentiment is determined using NLTK's VADER (Valence Aware Dictionary and sEntiment Reasoner), a lexicon and rule-based sentiment analysis tool specifically designed for text from social media but effective on product reviews as well.

### Workflow

1. Load and preprocess the dataset.
2. Split reviews into positive and negative subsets based on ratings.
3. Apply NLP preprocessing techniques to clean review texts.
4. Perform sentiment analysis using VADER to classify reviews.

## Usage

To replicate or extend this analysis:

* Install the required libraries using `pip install numpy pandas nltk`.
* Ensure NLTK datasets (`wordnet`, `stopwords`, `punkt`, and VADER lexicon) are downloaded.

## Results

The sentiment analysis effectively categorizes customer feedback into positive or negative groups, facilitating customer insight extraction and product improvement strategies.

## Potential Improvements

* Experiment with additional machine learning techniques like logistic regression or neural networks.
* Fine-tune preprocessing steps further, such as incorporating lemmatization or sentiment-specific vocabulary adjustments.

## License

This project is available for open use and adaptation.
