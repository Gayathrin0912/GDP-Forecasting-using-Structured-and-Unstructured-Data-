# GDP Forecasting with Structured and Unstructured Data using VAR and LLM-based Sentiment Analysis and Forecasting

This project explores the integration of structured economic & financial data and unstructured news data to forecast GDP trends. It leverages traditional time series forecasting models and modern NLP techniques, including Large Language Models (LLMs), for sentiment analysis.

---

## 📌 Project Overview

The objective is to improve GDP prediction accuracy by combining:

- **Structured data** (historical quarterly GDP values collected from WDB and yfinance)
- **Unstructured data** (news articles related to economy, agriculture, and industrial sectors)

The model evaluates if sentiment extracted from the news has a measurable impact on GDP and whether it can be incorporated into forecasting models like ARIMAX & VAR.

---

## 📂 Files and Structure

| File | Description |
|------|-------------|
| `GDP.ipynb` | Performs time series forecasting on structured GDP data and furthermore the forecasts of GDP together with the sentiment analysis scores of unstructured data.|
| `News_Articles_(Data_preprocessing).ipynb` | Preprocesses raw news articles using NLP techniques for LLM-based sentiment analysis. |
| `GDP_Prompts.ipynb` | Applies OpenAI LLMs to extract insights and economic sentiment from the preprocessed news. |
| `BigData_Project_Report.pdf` | Comprehensive project report including methodology, analysis, results, and conclusions. |

---

## 🔍 Key Features

### 1. **Structured Data Analysis**
- Time series modeling of quarterly GDP data using **VAR**.
- Data preprocessing and visualization.
- Stationarity testing (ADF test) and model evaluation using AIC/BIC values.
- Model performance validated with RMSE and comparison plots of actual vs predicted GDP.

### 2. **Unstructured Data Preprocessing**
- Collection of real-world news articles relevant to Indian economy.
- Text cleaning: stopword removal, lemmatization, and formatting.
- Use of custom keywords to filter and classify economic news by sector.

### 3. **Sentiment Analysis with LLMs**
- Prompts generated for LLMs (e.g., OpenAI GPT) to extract economic sentiment (positive/negative/neutral).
- Sector-wise sentiment aggregation for Agriculture, Industrial, and Service sectors.
- Fusion of sentiment trends with GDP modeling pipeline (conceptual and comparative).

---

## 📊 Results & Insights

- Sector-wise sentiment trends extracted from news correlate with known GDP events (e.g., dips during pandemic periods).
- Demonstrated that LLM-based sentiment analysis can enhance understanding of economic dynamics when combined with structured data.

---

## 🛠️ Tech Stack

- **Languages**: Python
- **Libraries**: pandas, matplotlib, statsmodels, OpenAI API
- **NLP Tools**: regex, GPT (for LLM sentiment extraction)
- **Visualization**: matplotlib, seaborn

---

## ⚙️ How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/gdp-forecasting-sentiment
   cd gdp-forecasting-sentiment

2. Install required Python packages
   Make sure you have Python 3.7+ installed, then run:

   ```bash
   pip install pandas numpy matplotlib seaborn statsmodels openai nltk

3. Add your OpenAI API key for sentiment analysis and GDP forecasting when using News_Articles_(Data_preprocessing).ipynb and GDP_Prompts.ipynb
