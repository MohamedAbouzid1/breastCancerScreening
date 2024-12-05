# Breast Cancer Screening with Neural Networks

This project aims to build a neural network model for breast cancer screening using a dataset that contains various features of cell nuclei from breast cancer biopsies. The goal is to classify whether the tumor is malignant or benign based on these features. The model is trained using PyTorch.

## Table of Contents
1. [Project Overview](#project-overview)
2. [Dataset](#dataset)
3. [Aim of the Project](#aim-of-the-project)
4. [Prerequisites](#prerequisites)
5. [Installation](#installation)
6. [Usage](#usage)
7. [Model Architecture](#model-architecture)
8. [Results](#results)
9. [License](#license)

## Project Overview

In this project, a neural network is trained to predict the class (malignant or benign) of breast cancer tumors using features extracted from digitized images of cell nuclei. The model is evaluated based on its ability to correctly classify tumors as malignant or benign. The dataset is split into training and testing sets, and the performance is tracked throughout the training process.

## Dataset

The dataset used in this project is a breast cancer screening dataset. Each row represents a tumor sample, and the features represent various measurements related to the cell nuclei of the tumor. These measurements include the radius, texture, perimeter, area, smoothness, compactness, concavity, and other shape-based features. 

Here are the first few rows of the dataset:

| mean radius | mean texture | mean perimeter | mean area | mean smoothness | ... | worst texture | worst perimeter | worst area | ... | target |
|-------------|--------------|----------------|-----------|-----------------|-----|---------------|-----------------|-----------|-----|--------|
| 17.99       | 10.38        | 122.80         | 1001.0    | 0.11840         | ... | 17.33         | 184.60          | 2019.0    | ... | 0      |
| 20.57       | 17.77        | 132.90         | 1326.0    | 0.08474         | ... | 23.41         | 158.80          | 1956.0    | ... | 0      |
| 19.69       | 21.25        | 130.00         | 1203.0    | 0.10960         | ... | 25.53         | 152.50          | 1709.0    | ... | 0      |
| 11.42       | 20.38        | 77.58          | 386.1     | 0.14250         | ... | 26.50         | 98.87           | 567.7     | ... | 0      |
| 20.29       | 14.34        | 135.10         | 1297.0    | 0.10030         | ... | 16.67         | 152.20          | 1575.0    | ... | 0      |


The **target** column contains the class labels:
- **0**: Benign
- **1**: Malignant

## Aim of the Project

The primary goal of this project is to:
1. Build a deep learning model to classify breast cancer tumors as benign or malignant using the features provided in the dataset.
2. Train a neural network using PyTorch, perform evaluation, and track the performance of the model.
3. Provide an accurate prediction system for breast cancer diagnosis that can assist healthcare professionals.

## Prerequisites

Before running this project, you will need the following libraries installed:

- `torch`: PyTorch for building and training the model.
- `scikit-learn`: For dataset splitting and evaluation.
- `numpy`: For numerical operations.
- `matplotlib`: For plotting results (if desired).
- `pandas`: For data manipulation and processing.

You can install the necessary dependencies using `pip`:

```bash
pip install torch scikit-learn numpy matplotlib pandas
