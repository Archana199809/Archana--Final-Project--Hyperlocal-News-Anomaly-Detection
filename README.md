## News Analysis & NLP Pipeline

This repository contains a comprehensive pipeline for processing, analyzing, and classifying news articles using advanced Natural Language Processing (NLP) and Machine Learning techniques. It transforms raw text into structured data with location extraction, sentiment analysis, topic modeling, and automated classification

## Key Features

**✓ Text Preprocessing & Cleaning**

The pipeline includes a robust cleaning function that uses Regular Expressions to remove non-alphabetic characters, standardizes text to lowercase, and utilizes NLTK for tokenization, stopword removal, and lemmatization

---
**✓ Geospatial Entity Extraction**

Using spaCy’s en_core_web_sm model, the system automatically identifies and extracts locations (GPE - Countries, Cities, States) from the text, ensuring a unique list of locations for each article

---
**✓ Sentiment Analysis**

The project integrates a specialized Transformer-based model (twitter-roberta-base-sentiment) to perform sentiment analysis, returning both a label (Negative, Neutral, Positive) and a confidence score for each article

---

**✓ Topic Modeling & Embeddings**

**Embeddings:** Generates dense vector representations of articles using the all-MiniLM-L6-v2 Sentence-Transformer model

**BERTopic:** Utilizes these embeddings to perform topic modeling, automatically identifying themes and assigning human-readable labels based on the most frequent words in each topic

---

**✓ Automated News Classification**

A dictionary-based classifier categorizes articles into six primary types—Crime, Festival, Business, Sports, Politics, and Technology—by matching keywords against the processed text

---

**✓ Anomaly Detection & ML Modeling**
The framework includes components for Anomaly Detection using IsolationForest and predictive modeling with the **XGBClassifier** to identify outliers or classify data based on extracted features

---

## Conclusion

The transition from raw data to an interactive Streamlit dashboard allows for real-time monitoring of news trends, making it a powerful tool for data-driven decision-making in the media and security sectors
.
## 💡 Practical Use Cases

The anomaly detection and classification capabilities of this project can be applied in several high-impact areas:

**✓Identifying Misinformation:**

By detecting statistical "anomalies" or outliers in reporting styles and topics, the system can flag potential fake news or highly unusual reports for manual verification

**✓Public Safety & Crisis Management:** 

The automated classification of "Crime" and "Politics" combined with location extraction allows authorities to monitor for sudden spikes in localized incidents or civil unrest

**✓Market & Business Intelligence:** 

Businesses can use the business classification and sentiment analysis to track unusual market shifts or competitor activity that deviates from established trends

**✓Automated News Aggregation:** 

News platforms can use the BERTopic modeling and keyword classification to automatically organize thousands of hyperlocal articles into searchable categories like Technology, Sports, and Festivals

**✓Sentiment Trend Tracking:**

NGOs or government bodies can monitor the "Sentiment Score" of hyperlocal news to gauge public reaction to new policies or local events in specific regions
