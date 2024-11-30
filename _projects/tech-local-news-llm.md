---
layout: project
title: Mapping Content Deserts&#x003A; Bridging Gaps in Local Journalism
date: 2000-12-31
categories: [Research, Machine Learning, Data Analysis]
links:
 paper: https://cplusj2024.github.io/papers/CJ_2024_paper_25.pdf
---

## Introduction

The rise of **"news deserts"** has brought attention to the severe consequences of diminishing local journalism, including increased polarization, unchecked corporate corruption, and societal disconnection. Building on this concept, this study introduces **"content deserts"**—geographic areas systematically underrepresented or entirely neglected by local press. Unlike news deserts, content deserts emphasize the **audience's perspective**, focusing on the unequal distribution of journalistic coverage within local regions.

To address this issue, this work leverages **open-source large language models (LLMs)** to identify locations mentioned in news articles and categorize them by topic and community information needs. The study evaluates the capabilities of these accessible tools for tagging local news content, ultimately proposing a framework for journalists to audit their reporting and better allocate resources to underserved areas.

## Methodology

### Data Collection
The study analyzed two diverse news outlets:  
- **The City**: 4,810 articles (2018–2024)  
- **The New York Post**: 94,776 articles (2018–2024)  
A control dataset of national news articles from 2019 was also included. Articles were sampled to ensure a broad range of topics and geographic coverage, with a particular focus on New York City boroughs.

### Annotation Tasks
Key tasks included:  
1. **Location Tagging**: Identifying all mentioned locations and the primary location for each article.  
2. **Topic Classification**: Categorizing articles by public interest topics.  
3. **Community Needs**: Determining if articles addressed community-specific information needs.  

### Model Selection and Evaluation
Three LLMs were tested:  
- **GPT-3.5-turbo**: Baseline private model  
- **Llama3-8B**: Open-source model  
- **Mistral3-7B**: Open-source model  

Models were evaluated using both static prompts and role-based prompts (e.g., a "local journalist" perspective). Human annotations served as ground truth, with discrepancies in location tagging resolved using **Google Maps API geocoding**.

### Exploratory Analysis
A larger sample of 1,000 articles (500 per publication) was analyzed using the best-performing LLM. Borough-specific coverage disparities were assessed, and thematic framing (e.g., crime coverage) was analyzed for potential biases.

## Key Findings

1. **Model Feasibility**:  
  Open-source LLMs like **Llama3** performed reliably in tagging article locations and topics but struggled with nuanced tasks, such as identifying specific communities mentioned.

2. **Geographic Disparities**:  
  Boroughs such as **Queens**, **the Bronx**, and **Staten Island** were significantly underrepresented compared to **Manhattan** and **Brooklyn**.

3. **Thematic Bias**:  
  Topics like **crime** were often framed negatively, underscoring potential biases in local reporting.

4. **Future Potential**:  
  While promising, the study highlights the need for fine-tuning models for local news-specific tasks to improve accuracy in identifying community needs.

## Next Steps

Tuning the prompt engineering on more updated large language models.

Meanwhile, we are developing an **auditing tool** to visualize the geographic distribution of news and social media topics across neighborhoods within a city. This tool incorporates demographic data, such as:  
- **Gender Ratio (M/F)**  
- **Median Age**  
- **Median Household Income**  
- **Poverty Rate**  
- **Education Levels**  
- **Median House Value**  
- **Health Insurance Coverage**  

These metrics enable a nuanced understanding of how journalistic content aligns with the characteristics and needs of different communities.

## Skills Highlighted

- Prompt Engineering  
- Survey Design  
- User Interview  
- Product Design  

## Publication

Paper Link: [Computation & Journalism Symposium 2024](https://cplusj2024.github.io/papers/CJ_2024_paper_25.pdf)  
Status: **Accepted**

## Collaborators

- Marianne Aubin Le Quéré, Cornell University  
- Tazbia Fatima, Hearst Newspapers  
- Michael Krisch, Brown Institute for Media Innovation