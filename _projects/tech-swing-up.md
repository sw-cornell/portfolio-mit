---
layout: project
title: SwingUp - Advancing Baseball Hitting Mechanics
date: 2024-01-01
categories: [Sports Analytics, Machine Learning, Web Development]
links:
 github: https://github.com/HerStat-Heroes/herstatheroes-mvp
 demo: https://herstatheroes-backend-67082157402.us-central1.run.app/
 presentation: https://drive.google.com/file/d/1sMIxXD4sa9SlaOfhLlElkON-pONQSv1_/view?usp=sharing
---

## Introduction

This project focuses on advancing the understanding and refinement of baseball hitting mechanics to provide actionable insights for athletes and coaches. The goal is to optimize the **squared-up rate**—the ratio of actual exit velocity to maximum possible exit velocity—serving as a key indicator of contact quality. The dataset, provided by the event organizers, comprises a year's worth of baseball swing data from **Minor League Baseball**.

## Technical Details

We employed a **Random Forest model** to categorize the squared-up rate into predefined ranges, inspired by MLB guidelines where "any swing that's at least 80% squared up is considered squared up." The categories are as follows:

- **Worst**: below 0.5
- **Bad**: 0.5 to 0.6
- **Pass**: 0.6 to 0.7
- **OK**: 0.7 to 0.8
- **Good**: 0.8 to 0.9

The model achieved the following metrics:
- **Accuracy**: 0.7937
- **Precision**: 0.8183
- **Recall**: 0.7937
- **F1 Score**: 0.7967

### Feature Engineering

Key features selected for prediction included:
- **Trajectory Length**: Calculated from the bat head's location data
- **Swing Speed**: Derived from the bat head's instantaneous speed at contact
- **Pitch Speed, Pitch Spin, and Hit Speed**: Directly provided in the dataset
- **Contact Point on the Bat**: Determined by the positional relationship between the bat and ball at contact
- **Stress Level**: A dynamic feature based on game conditions (outs, strikes, balls)

## Key Insights

1. **Trajectory Length**:
  Longer trajectories were unexpectedly associated with lower squared-up rates. This indicates that excessive swing movements may negatively impact hit power.

2. **Contact Point**:
  Analysis revealed that the ideal contact point lies between **20% and 40%** of the bat's length from the handle. Hits closer to the bat's head correlated with better exit velocity conversion rates.

3. **Hit Speed**:
  Strongly influenced exit velocity conversion rates, with higher hit speeds significantly improving outcomes.

4. **Stress Impact**:
  The effect of stress on performance remains inconclusive. Players responded differently under pressure, highlighting the need for further data collection and analysis.

## Digital Coaching System: Swing Up

To assist athletes in visualizing **ball and bat locations** for each pitch and maximize their squared-up rate, we developed a digital coaching system called **Swing Up**. The system offers insights at three levels:

- **By Team**: Enter the team ID to view all related hits
- **By Hitter**: Enter the hitter ID to view specific performance data
- **By Event**: Enter the pitch or hit event ID for detailed analysis

## Skills Highlighted
- Machine Learning
- Web Development
- Python
- Product Design

## Collaborators
- Mia Xuening Wang
- Yiran Li
- Mahira Pathan**