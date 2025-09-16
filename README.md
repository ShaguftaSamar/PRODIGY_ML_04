# Task-04:Develop a hand gesture recognition model that can accurately identify and classify different hand gestures from image or video data, enabling intuitive human-computer interaction and gesture-based control systems.

## Overview

This project implements **Task-04: Hand Gesture Recognition**, designed to accurately identify and classify different hand gestures from images or video data. The system enables **intuitive human-computer interaction** and **gesture-based control**, making it suitable for applications such as virtual interfaces, robotics, and accessibility tools.

The system uses **Convolutional Neural Networks (CNNs)** for gesture classification and supports both **image-based predictions** and **real-time webcam gesture detection**.

---

## Dataset

The dataset used for training and testing is the **LeapGestRecog dataset**:

[LeapGestRecog Dataset on Kaggle](https://www.kaggle.com/gti-upm/leapgestrecog)

**Details:**

* Contains images of **10 different hand gestures** performed by multiple users.
* Gestures include: Palm, L, Fist, FistMoved, Thumb, Index, OK, PalmMoved, C, Down.
* For faster training and experimentation, a **smaller dataset** was created with **200 images per gesture**.
* The smaller dataset is included in this repository as a **ZIP file (`leapGestRecog_small.zip`)**. Unzip it before running the project.

---

## Features

1. **Gesture Classification:** Accurately recognizes 10 different hand gestures.
2. **Real-Time Prediction:** Detects hand gestures using a webcam with a bounding box highlighting the hand.
3. **Model Evaluation:** Includes validation accuracy, confusion matrix, and classification report.
4. **Optional Test Set Evaluation:** Measures performance on an unseen test set of gestures.

---

## Implementation Summary

* **Data Preparation:** Images organized into class folders and sampled to 200 per gesture.
* **Model Architecture:** CNN with convolutional, pooling, dense, and dropout layers to achieve accurate classification.
* **Training:** Grayscale images resized to 64×64 pixels; trained with categorical cross-entropy loss.
* **Prediction:** Supports both **single image prediction** and **real-time webcam prediction** with confidence scores.

---

## Model Evaluation

* **Validation Accuracy:** Measured on a held-out subset of the dataset.
* **Confusion Matrix & Classification Report:** Evaluate per-class performance.
* **Test Set Accuracy (Optional):** Evaluates the model on unseen data for robustness.

---

## Results

* Achieved high accuracy on validation and test sets (typically >90%).
* Real-time gesture recognition works smoothly with bounding box visualization and confidence scores.

