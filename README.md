readme = r'''# X-Ray Image Classification Using CNN

This project uses a **Convolutional Neural Network (CNN)** to classify chest X-ray images into two categories:

- **NORMAL**
- **PNEUMONIA**

The model is built with **TensorFlow/Keras** and uses **OpenCV** for image preprocessing. Images are converted to grayscale, resized to **100 x 100**, normalized, and then passed through a deep CNN for training and prediction.

---

## Project Overview

The goal of this project is to build a deep learning model that can automatically analyze chest X-ray images and predict whether the image shows signs of **pneumonia** or is **normal**. This project demonstrates a complete image classification workflow including:

- loading and preprocessing image data,
- training a CNN model,
- evaluating model performance on test data,
- predicting individual X-ray images with confidence scores.

---

## Features

- Binary image classification: **Normal vs Pneumonia**
- Image preprocessing using **OpenCV**
- Deep CNN architecture with multiple convolutional layers
- Model training with **TensorFlow/Keras**
- GPU support (if available)
- Test set evaluation
- Single-image prediction with confidence output
- Visualization of prediction results using **Matplotlib**

---

## Tech Stack

- **Python**
- **TensorFlow / Keras**
- **OpenCV (cv2)**
- **NumPy**
- **Pandas**
- **Matplotlib**

---

## CNN Architecture

The model contains:

- **4 Convolutional Layers** with filters:
  - 64
  - 128
  - 256
  - 512
- **ReLU Activation** after each convolution
- **MaxPooling2D** layers for downsampling
- **Dropout Layers** to reduce overfitting
- **Flatten Layer**
- **Dense Hidden Layer**
- **Sigmoid Output Layer** for binary classification

Loss Function: **Binary Crossentropy**  
Optimizer: **Adam**  
Metric: **Accuracy**

---

## Dataset Structure

Make sure your dataset is organized like this:

```bash
chest_xray/
│
├── train/
│   ├── NORMAL/
│   └── PNEUMONIA/
│
├── test/
│   ├── NORMAL/
│   └── PNEUMONIA/
│
└── val/
    ├── NORMAL/
    └── PNEUMONIA/
