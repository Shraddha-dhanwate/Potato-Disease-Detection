# Potato Disease Detection

A deep learning model for detecting diseases directly on potato images (Early Blight, Late Blight, Healthy) using image classification.

## Overview

A computer vision project that detects diseases in potatoes using deep learning. The model classifies potato images into **Healthy**, **Early Blight**, or **Late Blight** categories.

## Features

* Image preprocessing and augmentation
* CNN or transfer learning-based model
* Training and evaluation scripts
* Prediction on new images

## Dataset

**Source:** PlantVillage Dataset (Potato subset)

Structure:

```
train/
 ├── Early_Blight/
 ├── Late_Blight/
 └── Healthy/
```

## Model

* Input size: 224×224
* Architecture: CNN / MobileNetV2
* Optimizer: Adam
* Loss: Categorical Crossentropy
* Metrics: Accuracy

## How to Run

1. Clone repo and install dependencies:

```bash
pip install -r requirements.txt
```

2. Train model:

```bash
python train.py
```

3. Predict:

```bash
python predict.py --image sample.jpg
```

## Results

* Accuracy: ~93% (example)

## Tools Used

TensorFlow, Keras, NumPy, OpenCV, Matplotlib

## Future Work

* Improve accuracy using more data
* Add Grad-CAM for explainability
* Deploy with Streamlit

