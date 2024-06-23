# License_Plate_Recognition_and_Detection

## Overview

This project focuses on the detection and recognition of license plates from vehicle images using deep learning models. It involves two main tasks:

1. __License Plate Detection__: Locating the license plate in an image.
2. __License Plate Recognition:__ Recognizing the text on the detected license plate.

The project leverages pre-trained models and custom neural network architectures for accurate detection and recognition.

## Table of Contents

* Project Structure
* Setup and Installation
* Data Preparation
* Training the Models
* Testing the Models
* Results and Evaluation

## Project Structure

```
License_Plate_Detection_Recognition/
│
├── data/
│   ├── license_plates_detection_train/
│   │   ├── image1.jpg
│   │   ├── image2.jpg
│   │   └── ...
│   ├── license_plates_recognition_train/
│   │   ├── image1.jpg
│   │   ├── image2.jpg
│   │   └── ...
│   ├── Licplatesdetection_train.csv
│   └── Licplatesrecognition_train.csv
│
├── test/
│   ├── image1.jpg
│   ├── image2.jpg
│   └── ...
│
├── output/
│   ├── SampleSubmission.csv
│
├── license_plate_recognition.ipynb
└── README.md
```

## Setup and Installation

Ensure you have Python 3.7+ installed. Install the necessary libraries using the provided below.

* tensorflow
* numpy
* pandas
* opencv-python
* matplotlib
* scikit-learn
* Pillow

## Data Preparation

### Detection Data

The __'Licplatesdetection_train.csv'__ file contains the bounding box coordinates for the license plates in the training images.

### Recognition Data

The __'Licplatesrecognition_train.csv'__ file contains the text labels for the license plates in the training images.

## Training the Models

### License Plate Detection

The detection model locates the license plate within an image. It uses the __'InceptionResNetV2'__ architecture for feature extraction, followed by a custom head for bounding box regression.

### License Plate Recognition

The recognition model identifies the text on the detected license plate. It also uses __'InceptionResNetV2'__ for feature extraction, followed by a fully connected layer for classification.

## Testing the Models

### Detection and Recognition Pipeline

The main pipeline detects license plates in test images and recognizes the text.

## Results and Evaluation

### Detection Results

The bounding boxes predicted by the detection model can be visualized to ensure accurate localization of license plates.

### Recognition Results

The recognized text from the license plates is printed out and can be compared with the ground truth for evaluation.
