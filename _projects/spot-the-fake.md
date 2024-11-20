---
layout: project
title: SpotTheFake - Detecting Fake Reviews
date: 2024-11-15
categories: [Technical, Machine Learning, Web Development]
technologies:
  - Python
  - Machine Learning
  - Streamlit
  - Natural Language Processing
  - Support Vector Machine
links:
  github: https://github.com/sw-cornell/SpotTheFake
---

## Overview

Fake reviews cost U.S. businesses nearly **$152 billion annually**, with one California-based business reporting a **25% drop in revenue** due to a competitor's fraudulent reviews. To address this growing concern, I collaborated with two students in my **Designing a Data Product** class at Cornell Tech to develop a **WebApp** aimed at protecting platforms, brands, and consumers from the damaging effects of fake reviews.

## Technical Implementation

The preprocessing phase was critical to the success of our model. We implemented several key strategies:

- **Stopword Removal**: Eliminated common but uninformative words (e.g., "and," "the")
- **Text Standardization**: Converted text to lowercase, removed extra whitespace, and cleaned special characters
- **Tokenization and Lemmatization**: Reduced dimensionality, aiding in feature extraction and enhancing model efficiency

The processed data led to more accurate predictions and minimized noise in the analysis. We developed a robust **Support Vector Machine (SVM)** classifier, achieving:

- **F1 Score**: 0.8659
- **AUC-ROC**: 0.9382

Key optimizations included:

- **Regularization Adjustments**: Tuned C = 0.5 to reduce overfitting and improve generalizability
- **Data Quality Enhancements**: Filtered out extreme-length reviews (less than 5 words or more than 300 words) to focus on informative samples

## Solution: Interactive WebApp

To showcase the model's capabilities, I built an interactive **web application using Streamlit**, allowing users to test the classifier with their own sample reviews. The app includes:

- **Real-Time Prediction**: Input a single comment to get an instant prediction on its authenticity
- **Review Exploration**: Analyze reviews for a specific place, view statistical analysis, and download detailed results for further review

This demo bridges the gap between technical implementation and user-friendly visualization, making the results easy to interpret.

![SpotTheFake Demo](../img/spotthefake-demo.jpg){:.responsive}

## Technology Stack

- **Machine Learning**: Support Vector Machine (SVM) classifier
- **Web Development**: Streamlit framework
- **Programming**: Python
- **Design**: Product Design principles

## Team

Project developed at Cornell Tech (NBAY 6170, Design Designing Products) in collaboration with:
- Chunbo Jie
- Mengtong He
- Ain Razali
- Nidhi Pavuluri