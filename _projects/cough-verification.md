---
layout: project
title: Exploring Cough Sounds for Gender Detection and Speaker Verification
date: 2024-03-15
categories: [Research, Machine Learning, Audio Processing]
technologies:
 - Wav2Vec
 - PyTorch
 - SpeechBrain
 - ECAPA-TDNN
 - Audio Processing
links:
 paper: ""
description: A research study exploring sequential cough recordings for enhanced speaker verification and gender detection using transformer models.
---

## Overview

Traditional speaker verification techniques rely heavily on structured speech data, while **non-speech sounds**, such as coughs, remain an underexplored avenue. Existing research on cough-based identity verification predominantly uses single cough sound recordings, limiting their applicability in real-world scenarios. This project explores the use of **sequential cough recordings** to enhance speaker verification systems.

## Project Details

### Collaboration
This project is a collaboration with the **Sean Parker Institute for the Voice** at Weill Cornell Medical College.

### Research Goals

#### 1. Gender Detection
- **Dataset:** Subset of the **Coswara dataset** (Aug 16, 2021 – Feb 24, 2022) with 800 user records (577 males, 233 females)
- **Preprocessing:** Normalization, silence removal, and uniform audio length
- **Model:** Wav2Vec transformer model
- **Results:**
 - Training accuracy: **88.3%** with an F1 score of **0.82**
 - Validation accuracy: **85%** with an F1 score of **0.76**

#### 2. Identity Verification
- **Dataset:** 2,746 cough recordings from 1,846 participants in the Coswara dataset
- **Model:** ECAPA-TDNN fine-tuned for cough-specific features using **SpeechBrain**
- **Metrics:**
 - **Equal Error Rate (EER):** Balanced false acceptance and rejection rates
 - **F1 Score:** Measured precision and recall for identity verification
- We achieved an EER of **15.22%** with an F1 score of **0.8559**

### Paper Status
This research is currently **under review**.

## Skills Highlighted
- Transformer Models (e.g., Wav2Vec)
- PyTorch

## Collaborators

- **Haomiao Li** – Cornell Tech
- **Linh He** – Sean Parker Institute for the Voice, Weill Cornell Medical College
- **Robin Zhao** – Sean Parker Institute for the Voice, Weill Cornell Medical College
- **Anaïs Rameau** – Sean Parker Institute for the Voice, Weill Cornell Medical College