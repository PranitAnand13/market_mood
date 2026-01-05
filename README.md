# Market Mood and Moves

## Overview

This repository contains the midterm progress for the *Market Mood and Moves* project
under the WiDS program. The work focuses on building and understanding a sentiment-driven
data pipeline that connects financial news with market data.

The emphasis so far has been on correct data handling, sentiment extraction, and
time alignment rather than on predictive modeling.

---

## Repository Structure

.
├── notebooks/
│   ├── 01_project_overview_and_architecture.ipynb
│   ├── 02_data_ingestion_and_storage.ipynb
│   ├── 02a_newsapi_data_ingestion.ipynb
│   ├── 03_text_processing_and_sentiment_engine.ipynb
│   └── 04_time_alignment_and_feature_preparation.ipynb
│
├── README.md
├── README_CONCEPTS.md
└── challenges

The notebooks also incorporate solutions to multiple **industry-style challenges**
introduced during the project.

---

## Notebook Summary

### 01_project_overview_and_architecture.ipynb
Introduces the problem motivation, outlines the overall pipeline, and explains how
news sentiment can be transformed into structured features for financial analysis.

---

### 02_data_ingestion_and_storage.ipynb
Demonstrates how raw news data can be structured and stored in a clean format.
Focuses on data hygiene and reproducibility. This notebook also addresses challenges
related to professional data storage practices.

---

### 02a_newsapi_data_ingestion.ipynb
Shows how financial news headlines can be collected programmatically using NewsAPI,
with secure handling of API keys and structured storage of responses.

---

### 03_text_processing_and_sentiment_engine.ipynb
Applies text preprocessing and sentiment analysis techniques to financial news.
A baseline lexicon-based sentiment model (VADER) is used, and the role of
finance-specific transformer models is discussed conceptually. Entity-based filtering
is explored to reduce noise from irrelevant news articles.

---

### 04_time_alignment_and_feature_preparation.ipynb
Handles one of the most critical aspects of financial data pipelines:
aligning news sentiment with market trading days. This notebook explicitly addresses
challenges such as timezone conversion, weekend handling, and prevention of
look-ahead bias through correct trading-day mapping and aggregation.

---

## Current Status

- News ingestion and storage implemented
- Sentiment extraction pipeline established
- Time alignment and aggregation completed
- Industry-style challenges related to data quality addressed
- Focus so far is on correctness and understanding rather than model performance

---

## Author

Pranit Anand
