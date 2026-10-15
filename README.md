# Digit Recognizer

Kaggle competition: [Digit Recognizer](https://www.kaggle.com/competitions/digit-recognizer)

**Score: 0.97639**

## Overview
Classify handwritten digits (0–9) from 28×28 grayscale images using a multilayer perceptron in PyTorch.

## Approach
- Loaded the data from CSV (784 pixel columns)
- Scaled pixels to 0–1
- Train/validation split (80/20)
- MLP: 784 → 128 → 64 → 10
- ReLU activations
- Adam optimizer + CrossEntropyLoss
- Mini-batch training with DataLoader

## Results
- Validation accuracy: ~97.7%
- Kaggle public score: **0.97639**

## Files
- `Digit_Recognizer.ipynb` — full notebook (data prep, training, evaluation, submission)

## Notes
This was done after Chapters 9–11 of *Hands-On Machine Learning with Scikit-Learn and PyTorch*.  
The model is a plain MLP (no convolutions). CNNs are covered in later chapters.
