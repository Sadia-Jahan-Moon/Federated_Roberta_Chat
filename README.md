# Privacy-Preserving Mental Health Detection Using Federated Learning

## Overview

This project presents a privacy-focused mental health detection system that identifies emotional states and psychological disorders from one-to-one chat messages using **Federated Learning (FL)**.

Traditional mental health detection systems require centralized data collection, which creates privacy risks. This project addresses this challenge by keeping user conversations on local devices and sharing only model updates during training.

A fine-tuned **RoBERTa-based classifier** is trained using Federated Learning to detect eight mental health categories.

## Mental Health Categories

The model classifies:

- Normal
- Sadness
- Stress
- Anxiety
- Depression
- Suicidal Intent
- Bipolar Disorder
- Personality Disorder

## Dataset

Dataset size:

- Training samples: 53,713
- Testing samples: 13,429

## Model Performance

The global federated model achieved:

| Metric | Score |
|--------|-------|
| Accuracy | 87.26% |
| Weighted F1 Score | 0.87 |
| Macro F1 Score | 0.85 |

## System Workflow

```
Private Chat Messages
          |
          v
 Text Preprocessing
          |
          v
 RoBERTa Classification Model
          |
          v
 Federated Learning Training
          |
          v
 Mental Health Prediction
```

## Key Features

- Privacy-preserving mental health detection
- Federated Learning-based model training
- RoBERTa transformer-based classification
- Detection of emotions and psychological disorders
- Real-time prediction using Flask web interface

## Technology Stack

### Machine Learning
- Python
- Transformers
- RoBERTa
- Federated Learning

### NLP
- Text preprocessing
- Tokenization
- Transformer-based text classification

## Privacy Approach

This project uses Federated Learning to protect sensitive user information:

- Raw chat data never leaves the user's device
- Only model parameters are shared
- A global model is created through federated aggregation

