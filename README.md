# Market Mood and Moves

## Overview

This repository contains the midterm-to-endterm progress for the *Market Mood and Moves*
project under the WiDS program (Analytics Club). The project explores how financial
news sentiment can be systematically processed and aligned with market data to form
a realistic sentiment-driven analytics pipeline.

The primary focus of the work has been on **data correctness, pipeline design, and
conceptual understanding**, rather than on optimizing predictive accuracy. Emphasis
has been placed on understanding how sentiment signals are generated, aligned in time,
and prepared for downstream modeling.

---

## Repository Structure

.
├── notebooks/  
│   ├── 01_project_overview_and_architecture.ipynb  
│   ├── 02_data_ingestion_and_storage.ipynb  
│   ├── 02a_newsapi_data_ingestion.ipynb  
│   ├── 03_text_processing_and_sentiment_engine.ipynb  
│   ├── 04_time_alignment_and_feature_preparation.ipynb  
│   ├── 05_finbert_sentiment_analysis.ipynb  
│   └── 06_lstm_sequence_modeling.ipynb  
│  
├── challenges/  
├── README.md  
├── README_CONCEPTS.md  

The notebooks collectively demonstrate the evolution of the pipeline from raw data
collection to temporally aligned sentiment-aware sequence modeling.

---

## Notebook Summary

### 01_project_overview_and_architecture.ipynb  
Introduces the project motivation from a behavioral finance perspective and outlines
the end-to-end pipeline. This notebook focuses on system design and explains how
financial news, sentiment signals, and market data interact within a unified framework.

---

### 02_data_ingestion_and_storage.ipynb  
Demonstrates structured handling of raw data, including schema design and storage
using formats such as SQLite. Emphasis is placed on data hygiene, reproducibility,
and separating raw data ingestion from downstream processing.

---

### 02a_newsapi_data_ingestion.ipynb  
Shows how financial news headlines are collected programmatically using NewsAPI.
The notebook covers secure API key handling, pagination limits, result caps in
free-tier plans, and structured storage of responses for later use.

---

### 03_text_processing_and_sentiment_engine.ipynb  
Introduces text preprocessing and sentiment extraction. A lexicon-based baseline
(VADER) is implemented to establish intuition, while the limitations of general
sentiment models for financial text are discussed. Entity-based filtering is explored
to reduce noise from ambiguous terms (e.g., “Apple” as a fruit vs. a company).

---

### 04_time_alignment_and_feature_preparation.ipynb  
Addresses one of the most critical challenges in financial modeling: correct temporal
alignment. News timestamps are mapped to trading days while handling market hours,
weekends, and timezones. This notebook explicitly focuses on preventing look-ahead
bias through careful alignment and daily aggregation of sentiment signals.

---

### 05_finbert_sentiment_analysis.ipynb  
Applies FinBERT, a domain-adapted transformer model, to extract probabilistic sentiment
scores from financial news. The notebook demonstrates how contextual embeddings improve
interpretation of financial language compared to general-purpose sentiment methods.

---

### 06_lstm_sequence_modeling.ipynb  
Introduces sequence modeling using LSTMs to capture temporal dependencies in market
data. Price-based features and aggregated sentiment signals are combined into sliding
windows to study how historical information influences future market behavior. The
focus remains on correct sequence construction rather than performance tuning.

---

## Industry-Style Challenges Addressed

Throughout the project, several realistic challenges were encountered and addressed:

- API rate limits and result caps in free-tier data sources  
- Ambiguity in financial language and entity identification  
- Timezone conversion and trading-day alignment  
- Look-ahead bias in sentiment-based financial pipelines  
- Data sparsity after strict filtering for company-specific news  

These challenges highlighted the gap between theoretical models and real-world data
constraints.

---

## Current Status

- News ingestion and structured storage implemented  
- Sentiment extraction using both baseline and domain-specific models  
- Temporal alignment and aggregation completed  
- LSTM-based sequence modeling explored  
- Emphasis placed on pipeline correctness, interpretability, and learning outcomes  

The repository reflects a learning-oriented approach, prioritizing conceptual clarity
and realistic system design over predictive performance.

---

## Author

**Pranit Anand**  
WiDS 5.0 – Analytics Club
