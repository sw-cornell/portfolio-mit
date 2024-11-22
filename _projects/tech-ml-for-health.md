---
layout: project
title: Predictive Model for Severe Menopause Symptoms Risk Factors (INFO 5375 Machine Learning for Health, Cornell Tech)
date: 2024-03-15
categories: [Healthcare, Machine Learning, Research]
technologies:
 - PyTorch
 - LSTM Networks
 - Random Forest
 - Support Vector Regression
 - Python
links:
 paper: https://drive.google.com/file/d/1L-JZ5sgsGPVx80oCglN9NaBUsY3HMpZ7/view?usp=sharing
 github: https://github.com/kevinwiranata/Menopredictor
---

## Introduction

Menopause is a critical life transition that impacts over 1.2 billion women globally, projected by 2030, with profound effects on their physical, emotional, and social well-being. Despite its significant impact, research on predicting the severity of menopause symptoms remains limited. Addressing this gap, this study explores how machine learning, specifically Long Short-Term Memory (LSTM) networks, can enhance the understanding and prediction of symptom severity based on lifestyle and health factors. By leveraging the longitudinal Study of Women's Health Across the Nation (SWAN) dataset, this work aims to bridge gaps in traditional statistical methodologies and offer personalized insights for managing menopause-related challenges.

## Technical Details

### Dataset
The SWAN dataset provides longitudinal data spanning multiple years, capturing physical, psychological, and social changes experienced by women during menopause. The final dataset included 2,802 unique patient records formatted into time-series sequences of six years, with 48 lifestyle indicators as input features and 47 menopause symptoms as target outputs.

### Model and Approach
The study employed an LSTM model, selected for its ability to process sequential data and identify temporal patterns. The architecture comprised an LSTM layer for sequence modeling, followed by a linear layer to output symptom severity predictions. Key innovations include:
- Tailored preprocessing to handle missing values (imputation via median/mode)
- Padding for uniform sequence lengths
- Cross-validation and hyperparameter tuning to optimize performance

Baseline models, including Random Forest and Support Vector Regression (SVR), were used for comparison. Model performance was evaluated using Mean Squared Error (MSE).

## Key Insights

1. **Model Performance**  
  The LSTM model achieved significantly lower MSE (3.938) compared to Random Forest (251.028) and SVR (236.612), highlighting its superior ability to model complex relationships in time-series data.

2. **Prediction Accuracy**
  - Biological symptoms (e.g., hormone-related metrics) were predicted with high precision
  - Emotional symptoms (e.g., loneliness, depression) posed greater challenges due to subjective variability
  - Physiologically complex metrics (e.g., diastolic blood pressure) exhibited the highest error rates

3. **Feature Attribution**
  Analysis using Captum Integrated Gradient scores revealed:
  - Physical symptoms were strongly influenced by specific lifestyle features, reflecting direct physiological pathways
  - Emotional symptoms were associated with a broader range of features, emphasizing their multifaceted nature

4. **Lifestyle Impacts**
  Lifestyle factors such as stress management and health routines emerged as critical determinants of symptom severity, offering potential avenues for targeted interventions.

## Conclusion

This study demonstrates the potential of LSTM networks in advancing the prediction of menopause symptom severity, outperforming traditional models by effectively capturing temporal dynamics in lifestyle and health data. The findings emphasize the importance of personalized care, with stress control and proactive health management identified as pivotal in mitigating symptom severity. While the work highlights the promise of machine learning in menopause research, challenges remain in addressing subjective variability and demographic imbalances. Future efforts should aim to incorporate more diverse datasets and clinical insights to refine models and enhance their applicability, paving the way for improved health outcomes for women worldwide.

## Skills Highlighted

- **Machine Learning**
- **PyTorch**
- **Literature Review**

## Collaborators

- **Zeming Guo**
- **Jueying Li**
- **Lisa Sam Wang**
- **Kevin Wiranata**