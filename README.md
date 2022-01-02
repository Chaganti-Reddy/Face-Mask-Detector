<h1 align="center">Face Mask Detection</h1>

<div align= "center"><img src="assets/4.jpg" width="250" height="250"/>
  <h4>Face Mask Detection System built with OpenCV, Keras/TensorFlow using Deep Learning and Computer Vision concepts in order to detect face masks in static images as well as in real-time video streams.</h4>
</div>

<div align="center">
    <!-- Python version -->
    <a href="https://www.python.org/"><img src="https://img.shields.io/badge/python-v3.8-blue?style=flat-square"/></a>
    <!-- Last commit -->
    <img src="https://img.shields.io/github/last-commit/achen353/Face-Mask-Detector?style=flat-square"/>
    <!-- Stars -->
    <img src="https://img.shields.io/github/stars/achen353/Face-Mask-Detector?style=flat-square"/>
    <!-- Forks -->
    <img src="https://img.shields.io/github/forks/achen353/Face-Mask-Detector?style=flat-square"/>
    <!-- Open Issues -->
    <a href="https://github.com/Chaganti-Reddy/Face-Mask-Detector/issues"><img src="https://img.shields.io/github/issues/achen353/Face-Mask-Detector?style=flat-square"/></a>
</div>

## Table of Contents
- [Features](#features)
- [About](#about)
- [Frameworks and Libraries](#frameworkslibraries)
- [Datasets](#datasets)
- [Training Results](#training-results)
- [Requirements](#requirements)
- [Setup](#setup) 
- [How to Run](#how-to-run)
- [License](#license)

## Features
- __Detection of multiple faces:__ able to detect multiple faces in one frame
- __Support for detection of improper mask wearing:__ our model is able to detect improper mask wearing including
  (1) uncovered chin, (2) uncovered nose, and (3) uncovered nose and mouth.
- __Alarm System for detecting without mask:__ our model is able to detect improper mask and gives an alarm to alert authorities.

## About
This app detects human faces and proper mask wearing in images and webcam streams. 

Under the COVID-19 pandemic, wearing
mask has shown to be an effective means to control the spread of virus. The demand for an effective mask detection on 
embedded systems of limited computing capabilities has surged, especially in highly populated areas such as public 
transportations, hospitals, etc. Trained on MobileNetV2, a state-of-the-art lightweight deep learning model on 
image classification, the app is computationally efficient to deploy to help control the spread of the disease.

While many work on face mask detection has been developed since the start of the pandemic, few distinguishes whether a
mask is worn correctly or incorrectly. Given the discovery of the new coronavirus variant in UK, we aim to provide a 
more precise detection model to help strengthen enforcement of mask mandate around the world.

## Frameworks and Libraries
- __[OpenCV](https://opencv.org/):__ Computer vision library used to process images
- __[OpenCV DNN Face Detector](https://github.com/opencv/opencv/blob/3.4.0/samples/dnn/resnet_ssd_face_python.py):__ 
  Caffe-based Single Shot-Multibox Detector (SSD) model used to detect faces
- __[Tensorflow](https://www.tensorflow.org/) / [Keras](https://keras.io/):__ Deep learning framework used to build and train our models
- __[MobileNet V2](https://arxiv.org/abs/1801.04381):__ Lightweight pre-trained model available in Keras Applications; 
  used as a base model for our transfer learning
- __[Numpy](https://numpy.org/):__ 
  Caffe-based Single Shot-Multibox Detector (SSD) model used to detect faces

## Datasets
The dataset used can be downloaded here - [Click to Download](https://github.com/chandrikadeb7/Face-Mask-Detection/tree/master/dataset)

This dataset consists of __7388__ images:
- `face_no_mask`: 3,846 images
- `face_with_mask`: 3,542 images

Each image is a cropped real-world face image of unfixed sizes.

The images used were real images of faces wearing masks. The images were collected from the following sources:

* __Kaggle datasets__ ([See here](https://www.kaggle.com/))
* __RMFD dataset__ ([See here](https://github.com/X-zhangyang/Real-World-Masked-Face-Dataset))