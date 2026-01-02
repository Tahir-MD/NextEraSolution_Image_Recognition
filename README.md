# 🖼️ Image Recognition with CNN - NextEra Internship Task

## 📌 Project Overview
This project implements a **Convolutional Neural Network (CNN)** for image classification using the **CIFAR-10 dataset**. The model is built with TensorFlow/Keras and trained to recognize 10 object categories.

## 🎯 Task Objective
- Build and train a CNN model for image recognition.
- Achieve maximum accuracy on the CIFAR-10 test set.
- Document the process and results.

## 📊 Dataset
**CIFAR-10 Dataset:**
- 60,000 32x32 color images
- 10 classes: airplane, automobile, bird, cat, deer, dog, frog, horse, ship, truck
- 50,000 training images, 10,000 test images

## 🏗️ Model Architecture
```python
Sequential([
    Conv2D(32, (3,3), activation='relu', input_shape=(32,32,3)),
    MaxPooling2D((2,2)),
    Conv2D(64, (3,3), activation='relu'),
    MaxPooling2D((2,2)),
    Conv2D(64, (3,3), activation='relu'),
    Flatten(),
    Dense(64, activation='relu'),
    Dense(10, activation='softmax')
])
