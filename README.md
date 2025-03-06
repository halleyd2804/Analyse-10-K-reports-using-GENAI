# Analyse-10-K-reports-using-GENAI
## Overview


---

## Table of Contents

1. [Dataset](#dataset)
2. [Models](#models)
 
---

## Dataset
The dataset consists of 10-K reports from 10 publicly traded companies. The data includes the following:
- **Company Name**: Amazon, Google, IBM, Meta, Microsoft, NVDIA, Oracle, Tesla, Salesforce, INTEL.
- **Content of 10-K Reports**: Full reports, including financial performance, risks, and other relevant information.

**Associated Data Files:**
- `10k_extracted_info.csv`: A CSV file containing extracted info summaried by Gemini.
- `my_AI_sentiment_ranking.txt`: A text file containig sentimental analysis of each ticker of Gemini.

---

## Models
The primary goal of this project is to perform **sentiment analysis and report summarization** on the 10-K reports using the **Gemini API**. The project uses the following approaches:
1. **Text Preprocessing**:
   - **Regex**: Regular expressions are used to extract relevant sections of the 10-K reports (such as opportunities, risk, and investment).
   - **BeautifulSoup**: Remove HTML tags from the text gathered.

2. **Gemini API Integration**:
   - The **Gemini API** is called to analyze the text data and generate a sentiment score for each report.
   - The sentiment score is classified into three categories: **bullish**, **bearish**, or **neutral**, based on the context of the report.

3. **Sentiment Analysis**:
   - Based on the analysis from the Gemini API, each report is assigned a sentiment label (bullish, bearish, or neutral).
   - The sentiment labels are then aggregated to predict the overall market sentiment for each company.


