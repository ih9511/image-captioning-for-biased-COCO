# Investigating Differences in CNN Models by Data Bias Based on Positive and Negative Images

## Overview
This project explores the impact of data bias on CNN models, specifically focusing on how positive and negative image data influence model performance. The research was presented at the Fall Conference of the Korean Society for Human Engineering in 2022 by Inheon Choi and Sangwon Lee.

## Table of Contents
1. [Background](#background)
2. [Objective](#objective)
3. [Methodology](#methodology)
4. [Result Analysis](#result-analysis)
5. [Discussion](#discussion)

## Background
### AI Embedded Services
The advancement of AI technology has led to its application in various fields, from chatbots to healthcare. As AI services and content continue to expand, the need for ethical AI has become increasingly important.

### AI for Humanity
In December 2020, the Ministry of Science and ICT and the Korea Information Society Development Institute established AI ethics guidelines based on three principles: human dignity, public interest, and technical suitability. These guidelines emphasize the need to address bias in AI models to ensure diversity and fairness.

### Biased AI
AI models trained on biased data can produce harmful outcomes, highlighting the importance of understanding how data bias affects model performance. This study aims to raise awareness of data bias and promote unbiased AI design through algorithmic interpretation.

## Objective
The objective of this study is to create two datasets with positive and negative biases and train the same CNN model on each dataset. By using CNN visualization techniques, we aim to visually confirm how each model learns biases, thereby providing insights into avoiding biased AI design.

## Methodology
![image](https://github.com/ih9511/image-captioning-for-biased-COCO/assets/46120405/e26de6ce-24ac-46d1-91ac-0aac0c151075)

### Dataset
#### AffectNet
AffectNet is a dataset containing approximately 450,000 facial expression images labeled with eight emotion categories: happy, surprise, neutral, sad, fear, disgust, anger, and contempt. The dataset is used to create three subsets: positive, negative, and neutral.

#### Data Separation
The data was restructured into three labels: positive (happy, surprise), neutral, and negative (sad, fear, disgust, anger, contempt). Each subset contained 30,000 images for positive, neutral, and negative data.

### Model
#### EfficientNet
EfficientNet was chosen due to its high accuracy and computational efficiency. The EfficientNet-B2 model was used as it provided the best accuracy on the AffectNet dataset.

### Visualization
#### CNN Visualization
CNN visualization techniques, such as LayerCAM, were used to identify the regions of images that the models focused on during classification. This helps in understanding how different biases in the training data influence model predictions.

## Result Analysis
### Neutral Image LayerCAM
The visualizations show how the positively biased model and the negatively biased model interpret neutral images differently.

### Positive Image LayerCAM
Differences in model interpretation for positive images highlight the impact of data bias on model learning.

### Negative Image LayerCAM
The analysis of negative images further demonstrates how data bias affects model predictions.

## Discussion
This study reveals that data bias significantly influences CNN models, which can be visually confirmed through LayerCAM visualizations. The findings emphasize the importance of using balanced datasets to train unbiased AI models, contributing to the development of ethical AI systems.
