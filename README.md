# AskAdam: An LLM-Powered Q&A Agent for NBA Analytics 🏀💻🔍

## Overview
AskAdam is an intelligent question-answering system that combines large language models (LLMs) with advanced basketball analytics to deliver fast, insightful responses to natural language queries. Built for analysts, coaches, fans, and data scientists, AskAdam bridges the gap between raw NBA data and actionable insights. AskAdam is built on NBA Team Data, consisting of data from the 2017/2018 season through midseason of the 2024/2025 season (excluding the 2020/2021 season).

## Features
- **Natural Language Understanding**
    Ask complex basketball questions in plain English — no SQL or code required.
- **LLM-Driven Intelligence**
    Powered by a large language model that interprets and responds to questions with contextual understanding and reasoning.
- **Advanced Basketball Analytics**
    Leverages real NBA data and statistical models to answer questions involving shot probabilities, player tendencies, team matchups, and more.
- **Real-Time Insight Delivery**
    Fast responses backed by efficient querying and processing pipelines.

## Example Questions
*"Which 5 teams led the league in scoring during the 22/22 season?"*

*"Which team leads the league in offesnsive efficiency this year, which team is last in offensive efficiency this year, and what is the difference between the two?"*

*"What was the Lakers record in 2022/2023 compared to their record in 2019/2020? What was the difference in games won?"*

AskAdam understands these questions and delivers clear, data-rich answers.  

## How It Works
- **Query Parsing** – Natural language queries are parsed and interpreted using an LLM.
- **Intent Recognition** – AskAdam identifies the user's intent (e.g., team comparison, team stats, historical trend).
- **Data Retrieval** – Relevant NBA data is extracted from https://www.nbastuffer.com.
- **Analytical Reasoning** – The model applies basketball-specific analytics to generate insights.
- **Response Generation** – A human-readable answer is generated.


## Methodology
- **Data Cleaning & Preprocessing:** Webscraped https://www.nbastuffer.com to retrieve relevant team data (data_prep.py)
- **Feature Engineering:** Utilized Azure's OpenAI Service to embed data and create vectorized dataframe (vectorize_data.py)
- **Generate LLM Response:** Utilized Azure's OpenAI service to generate sql queries, define prompts, and generate LLM Response (master_agent.py)

## Tech Stack
Python  
Azure OpenAI  
Pandas, NumPy, SQL, BeautifulSoup  
Vector Database (Azure Embeddings) for semantic search  

## Future Improvements
- Working to get this model stood up as an app or on a dedicated website
- Additional data can be implement: player data, fan data, sponsorship data, etc.

