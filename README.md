# Market Mood and Moves

## About

This project implements a structured pipeline for analyzing financial
news sentiment and aligning it with market data. The work focuses on
processing unstructured news text and preparing sentiment-based features
for financial analysis.

This project is part of the **WiDS Market Mood and Moves** program.

---

## Project Structure

.
├── notebooks/
│   ├── 01_project_overview_and_architecture.ipynb
│   ├── 02_data_ingestion_and_storage.ipynb
│   ├── 02a_newsapi_data_ingestion.ipynb
│   ├── 03_text_processing_and_sentiment_engine.ipynb
│   └── 04_time_alignment_and_feature_preparation.ipynb
│
├── README.md


---

## What Has Been Implemented

- Structured storage of news data  
- Secure ingestion of news using NewsAPI  
- Text preprocessing and sentiment analysis  
- Conversion of sentiment into numerical scores  
- Timezone-aware alignment of news with trading days  
- Aggregation of daily sentiment features  
- Merging of sentiment features with market data  

---

## Notes

- The project emphasizes clarity and correctness of the data pipeline.
- All steps are implemented in a modular notebook structure.
- Live API usage is limited to ensure reproducibility.

---

## Author

Pranit Anand
