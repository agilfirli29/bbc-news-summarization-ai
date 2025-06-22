# BBC News Summarization using IBM Granite (Capstone Project - Student Development Initiative IBM X Hacktiv8)

🚀 AI-powered summarization of BBC News articles using IBM Granite (Granite-3.3-8B-Instruct) via Replicate API.  
Includes EDA, visualization, LLM summarization, and insight extraction.

---

## 📌 Project Overview

This project aims to analyze and summarize BBC News articles using the IBM Granite large language model (LLM) via Replicate API. The goal is to understand how effectively AI can compress and summarize large articles into concise, meaningful summaries that can assist in content curation and news analysis.

---

## 📊 Dataset

- **Dataset Name**: BBC News Summary Dataset  
- **Source**: [Kaggle Dataset](https://www.kaggle.com/datasets/dignity45/bbc-news-summarycsv-format)
- **Description**: 2,225 BBC News articles with human-written summaries  
- **Columns**:
  - `Text`: Full news article
  - `Summary`: Human-written summary of the article

---

## 🧪 Analysis Process

1. **Data Preprocessing**  
   - Load dataset, clean null values, keep relevant columns

2. **Exploratory Data Analysis (EDA)**  
   - Analyze article lengths, generate WordCloud

3. **Summarization with IBM Granite**  
   - Use model `ibm-granite/granite-3.3-8b-instruct` via Replicate API  
   - Provide prompt for summarizing each article  
   - Configure parameters (max_tokens, top_p, etc.)

4. **Insight Comparison**  
   - Compare generated summaries with original human summaries

---

## 🧠 Insight & Findings

- IBM Granite provides fluent, relevant one-paragraph summaries.
- Best results are obtained with prompt tuning and token limitations.
- Summaries often retain the essence, although minor factual details may vary.

---

## 💡 Recommendations

- IBM Granite is effective for summarizing large text datasets.
- Useful for news curators, researchers, and information systems.
- AI output should be reviewed for factual accuracy in critical use cases.

---

## 🤖 AI Support Explanation

- **Model**: `ibm-granite/granite-3.3-8b-instruct`  
- **Platform**: [Replicate.com](https://replicate.com/ibm-granite/granite-3.3-8b-instruct)  
- **Prompt Example**:
- **Parameters Used**:
```python
{
    "top_k": 0,
    "top_p": 1.0,
    "max_tokens": 256,
    "repetition_penalty": 1.0
}
