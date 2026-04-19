Liver Cancer Detection using Deep Learning

This repository contains the implementation and experimental results of multiple deep learning models for liver cancer detection using CT scan images.
The goal is to evaluate different architectures and compare their performance under different data splits.

📌 Overview

In this project, several modern deep learning models are trained and evaluated on liver CT scan images to detect the presence of tumors.

We experimented with:

Different model architectures
Different data splits (70/30 and 75/25)
Multiple evaluation metrics and visualizations

The repository is organized in a way that makes it easy to understand the full workflow from training to evaluation.

🧠 Models Used

The following models are implemented and tested:

EfficientNetV2-S
ConvNeXt-Tiny
Swin Transformer
MobileViT-S

Each model has its own notebook for training and evaluation.

⚙️ Workflow

The overall pipeline followed in this project:

Data Preparation
CT scan images are collected and organized
A small sample dataset is included in this repo for demonstration
Preprocessing
Image resizing
Normalization
Conversion to tensor format

Data Splitting
70% training / 30% testing
75% training / 25% testing

Model Training
Models are trained using the prepared dataset
Performance is tracked across epochs

Evaluation
Accuracy
Precision
Recall (Sensitivity)
F1-score
ROC-AUC
Specificity

Visualization
ROC Curve
F1 Score progression
Accuracy & Loss curves
Confusion Matrix


📂 Project Structure
data/
 ├── sample/                # Small set of images (for demo)
 
notebooks/
 ├── convnext-tiny 70,30 split.ipynb
 ├── convnext-tiny 75,25 split.ipynb
 ├── convnext-tiny.ipynb
 ├── efficientnetv2-s 70,30 split.ipynb
 ├── efficientnetv2-s 75,25 split.ipynb
 ├── efficientnetv2-s.ipynb
 ├── mobilevit-s.ipynb
 └── swin-transformer.ipynb

results/
 ├── ConvNeXt-Tiny/
 │   ├── 70-30 split/
 │   └── 75-25 split/
 │
 ├── efficientnetv2-s/
 │   ├── 70-30 split/
 │   └── 75-25 split/

Each result folder contains:
ROC curve
F1-score curve
Accuracy & Loss curves
Confusion matrix
Validation summary table


📦 Dataset

Due to size limitations (~3.6GB), the full dataset is not included in this repository.

Instead:
A small sample (15 images) is provided in data/sample/
This is only for demonstration and structure understanding

To reproduce the full results:
Download the dataset from: https://www.kaggle.com/datasets/ag3ntsp1d3rx/litsdataset2/data
Place it inside


📎 Conclusion

This project demonstrates how different deep learning architectures perform on liver cancer detection tasks.
The results indicate that models like EfficientNetV2-S achieve very high performance, making them strong candidates for medical image classification tasks.
