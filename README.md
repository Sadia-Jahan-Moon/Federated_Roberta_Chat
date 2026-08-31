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
## Publication

This project is based on the IEEE conference paper:

**A Privacy-Focused Classification System for Monitoring Mental Health in One-to-One Chat**

Published in:

**2025 28th International Conference on Computer and Information Technology (ICCIT)**  
IEEE Xplore, 2025


**DOI:**  
https://doi.org/10.1109/ICCIT68739.2025.11491280

## How to Cite This Work

If you use this project or refer to this research, please cite:

> S. J. Moon, M. A. Rahman, F. Hossain, and M. A. Hannan, "A Privacy-Focused Classification System for Monitoring Mental Health in One-to-One Chat," *2025 28th International Conference on Computer and Information Technology (ICCIT)*, Cox's Bazar, Bangladesh, 2025, pp. 3824-3829, doi: 10.1109/ICCIT68739.2025.11491280.

**Keywords:** Federated learning, mental health detection, non-IID data, one-to-one private chat, privacy-preserving machine learning, natural language processing.



