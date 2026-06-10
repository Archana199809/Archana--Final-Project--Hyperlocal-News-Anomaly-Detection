## 🌎 News Analysis & NLP Pipeline

This repository contains a comprehensive pipeline for processing, analyzing, and classifying news articles using advanced Natural Language Processing (NLP) and Machine Learning techniques. It transforms raw text into structured data with location extraction, sentiment analysis, topic modeling, and automated classification

## 🚀Key Features

**⚙️ Text Preprocessing & Cleaning**

The pipeline includes a robust cleaning function that uses Regular Expressions to remove non-alphabetic characters, standardizes text to lowercase, and utilizes NLTK for tokenization, stopword removal, and lemmatization

---
**📍 Geospatial Entity Extraction**

Using **spaCy’s en_core_web_sm model**, the system automatically identifies and extracts locations (GPE - Countries, Cities, States) from the text, ensuring a unique list of locations for each article

---
**🧠 Sentiment Analysis**

The project integrates a specialized Transformer-based model **RoBERTa**-base-sentimenT to perform sentiment analysis, returning both a label (Negative, Neutral, Positive) and a confidence score for each article

---

**🧬 Topic Modeling & Embeddings**

**Embeddings:** Generates dense vector representations of articles using the all-MiniLM-L6-v2 **Sentence-Transformer** model

**BERTopic:** Utilizes these embeddings to perform topic modeling, automatically identifying themes and assigning human-readable labels based on the most frequent words in each topic

---

**📂 Automated News Classification**

A dictionary-based classifier categorizes articles into six primary types—**Crime, Festival, Business, Sports, Politics, and Technology**—by matching keywords against the processed text

---

**🚨 Anomaly Detection & ML Modeling**

The framework includes components for Anomaly Detection using **IsolationForest** and predictive modeling with the **XGBClassifier** to identify outliers or classify data based on extracted features

---

## ✅ Conclusion:

The transition from raw data to an interactive Streamlit dashboard allows for **real-time monitoring** of news trends, making it a powerful tool for data-driven decision-making in the media and security sectors

## 💡 Practical Use Cases

**🚨 Public Safety & Law Enforcement:** By combining the auto-classification of "**crime**" keywords with spaCy’s geospatial entity extraction, authorities can identify unusual spikes in localized incidents (like "shooting" or "robbery") in specific cities or regions

**📉 Market & Business Intelligence:** Organizations can use the **RoBERTa**-based sentiment analysis to monitor the "Business" category. Detecting negative sentiment anomalies or outliers in "acquisition" or "revenue" reports can provide an early warning for market volatility.

**🗞️ Smart News Aggregation:** Using BERTopic and Sentence-Transformers, news platforms can automatically organize thousands of hyperlocal articles into coherent topic labels. This allows for the creation of personalized news feeds based on specific **user interests** like Technology, Sports, or Politics.

**🛡️ Misinformation & Fact-Checking:** The Anomaly Detection (**XGBoost**) component can flag articles that deviate significantly from standard reporting patterns. These "**outliers**" can be prioritized for manual verification to identify potential fake news or propaganda.

**📍 Localized Crisis Management:** The system’s ability to **extract locations** (GPE) and monitor "NewsType" trends allows NGOs or government agencies to track developing local emergencies, such as sudden shifts in reporting about "festivals" or "government" policy in specific districts

**📊 Public Sentiment Analysis:** By tracking sentiment scores across different "NewsTypes," researchers can gauge the collective public mood regarding "Politics" or "Technology" within a s**pecific timeframe**, visualized through the **Streamlit dashboard**.

