# MIE1517HW2---Hand Gesture Recognition (ASL A–I) with CNN + Transfer Learning

This repo contains my Assignment 2 work on hand gesture recognition. The goal is to classify American Sign Language letters A to I using a dataset of hand images and a convolutional neural network.

## What’s inside
- Part A: Collect and clean a small image dataset (ASL A–I)
- Part B: Train a CNN classifier and evaluate performance
- Bonus: Use transfer learning (AlexNet feature extraction) to improve test accuracy

## Key ideas
- Subject based split to prevent data leakage (images from the same person stay in only one split)
- CNN trained from scratch, then improved with transfer learning
- Evaluation includes test accuracy, confusion matrix, and per class precision, recall, and F1

## Results (high level)
- CNN from scratch: test accuracy around 75.7%
- Transfer learning with AlexNet features: test accuracy around 80.1%
- Most confused gestures: G and H (visually similar in the dataset)

## Tech stack
Python, PyTorch, NumPy, scikit learn, matplotlib (Google Colab friendly)

## How to run
1. Open the notebook (or run the exported HTML logic in Colab/Jupyter)
2. Place your cleaned gesture images in the expected folder structure
3. Run cells in order: data prep → split → train → evaluate → transfer learning

## Notes
This project is built for learning and clean evaluation. The split strategy is designed to avoid inflating accuracy by leaking similar images across train and test.
