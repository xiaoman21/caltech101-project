# Caltech-101 Image Classification Project

This repository contains experiments for multi-class image classification on the Caltech-101 dataset.  
We compare a classical machine learning baseline (HOG + Linear SVM) with deep learning transfer-learning models (ResNet-18 and EfficientNet-B0), and conduct ablation studies on the best-performing model.

## Project Overview

**Models**
- Classical baseline: HOG features + Linear SVM
- Deep learning: ResNet-18 (ImageNet pretrained)
- Deep learning: EfficientNet-B0 (ImageNet pretrained)

**Ablation Studies (EfficientNet-B0)**
- Input resolution: 128×128 vs 64×64
- Data augmentation: with vs without augmentation

**Evaluation Metrics**
- Overall accuracy
- Per-class accuracy
- Confusion matrix
- Precision / Recall / F1-score (macro and weighted averages)

## Dataset

We use the Caltech-101 dataset (101 object categories; ~9,000 images).  
This repo does **not** include the dataset files.

Download (Kaggle):
- https://www.kaggle.com/datasets/imbikramsaha/caltech-101

After downloading and extracting, place the dataset under:
data/raw/caltech-101/


> Note: If you see a folder like `BACKGROUND_Google`, it is typically excluded to keep exactly 101 classes.

## Repository Structure


caltech101-project/
│
├── notebooks/ # notebooks for data split, models, and ablations
├── outputs/ # generated outputs (figures, logs)
├── report/ # final report PDF and figures
├── data/ # dataset folder (ignored by git)
│
├── requirements.txt # python dependencies
├── .gitignore
└── README.md

