# ASL Hand Gesture Recognition with CNN and Transfer Learning

## Overview

This project classifies American Sign Language hand gestures for the letters A through I. It compares a convolutional neural network trained from scratch with transfer learning based on AlexNet features.

## Data Preparation

- Collected and cleaned hand-gesture images for nine ASL classes
- Organized images by subject and gesture
- Used a subject-based train/validation/test split so images from the same person do not appear across different splits
- Applied preprocessing suitable for CNN training and transfer learning

## Methodology

- Trained a CNN classifier from scratch
- Extracted pretrained AlexNet features for transfer learning
- Evaluated both approaches using accuracy, confusion matrices, precision, recall, and F1 score
- Analyzed errors across visually similar gesture classes

## Key Results

- CNN trained from scratch: approximately 75.7% test accuracy
- AlexNet transfer learning: approximately 80.1% test accuracy
- Transfer learning improved generalization over the baseline CNN.
- Gestures G and H produced the most confusion because of their visual similarity in the dataset.

## Technologies

Python, PyTorch, AlexNet, transfer learning, NumPy, scikit-learn, matplotlib

## How to Run

1. Open the project notebook in Jupyter Notebook or Google Colab.
2. Place the cleaned gesture images in the expected folder structure.
3. Run the workflow in order: preprocessing, subject-based splitting, training, evaluation, and transfer learning.
