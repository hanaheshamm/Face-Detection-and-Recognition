# Face-Detection-and-Recognition

## Overview
This project implements a comprehensive system for face detection and recognition using the Haar cascade classifier for face detection and the Eigenfaces method for face recognition. The system is designed to identify and recognize faces in images, leveraging OpenCV and Principal Component Analysis (PCA).

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
  - [Face Detection](#face-detection)
  - [Face Recognition](#face-recognition)
- [Evaluation](#evaluation)
  - [ROC Curve](#roc-curve)
- [Results](#results)
- [Installation](#installation)

## Introduction
This project involves the detection and recognition of faces in images using machine learning and computer vision techniques. It employs OpenCV for implementing the Haar cascade classifier for detecting faces and uses PCA for recognizing faces through the Eigenfaces method.

## Features
### Face Detection
- **Haar Cascade Classifier**:
  - Utilizes OpenCV's pre-trained Haar cascade classifier for detecting faces.
  - Efficiently detects faces in images with varying scales and lighting conditions.
  - Implements the `detectMultiScale` function for scanning the image at multiple scales.

- **Bounding Boxes**:
  - Draws rectangles around detected faces for visual confirmation.
  - Adjustable parameters such as `scaleFactor`, `minNeighbors`, `minSize`, and `maxSize` for tuning detection accuracy.

### Face Recognition
- **Eigenfaces Method**:
  - Applies Principal Component Analysis (PCA) to reduce the dimensionality of face images.
  - Projects faces into a lower-dimensional eigenface space capturing the most significant facial features.
  - Robust to variations in lighting, expressions, and minor occlusions.

- **Training and Testing**:
  - Organizes training images into a matrix for PCA computation.
  - Projects test images into the eigenface space and performs recognition by comparing with training images.

### Evaluation
- **ROC Curve Analysis**:
  - Evaluates the performance of the face recognition system.
  - Plots the True Positive Rate (TPR) against the False Positive Rate (FPR) for different thresholds.
  - Calculates Area Under the Curve (AUC) for an aggregate measure of performance.

## Results
### Face Detection Results
![Face Detection Result](https://github.com/hanaheshamm/Face-Detection-and-Recognition/assets/115111861/54d857fb-5571-48b5-bbfc-dfb786dbe13a)

### Recognition Results
![Recognition Result 1](https://github.com/hanaheshamm/Face-Detection-and-Recognition/assets/115111861/48fbe1a7-f5c6-401c-aab7-6460d6e40f6a)
![Recognition Result 2](https://github.com/hanaheshamm/Face-Detection-and-Recognition/assets/115111861/bab43e5f-5e40-4dc9-ab94-08d951769973)
![Recognition Result 3](https://github.com/hanaheshamm/Face-Detection-and-Recognition/assets/115111861/92ddb206-7b8a-48e8-8c7e-2dcd667a3e59)

### Roc Results
![image](https://github.com/hanaheshamm/Face-Detection-and-Recognition/assets/115111861/0d3df79a-bc61-48f4-b17e-54e93aeaad9e)
![image](https://github.com/hanaheshamm/Face-Detection-and-Recognition/assets/115111861/c02cd655-d22b-4015-9ceb-efc7fe2d2479)

![image](https://github.com/hanaheshamm/Face-Detection-and-Recognition/assets/115111861/72c1e639-5ab2-49a3-9650-f7db1b318dac)


## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/hanaheshamm/face-detection-recognition.git
   cd face-detection-recognition
