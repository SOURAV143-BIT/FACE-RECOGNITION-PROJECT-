# FACE-RECOGNITION-PROJECT-

# Face Detection Using OpenCV Haar Cascade Classifier

## Project Overview

This project demonstrates how to detect human faces in images using OpenCV's Haar Cascade Classifier. The system automatically scans images stored in a directory, identifies faces, and displays the detected faces with bounding boxes.

## Objectives

* Detect human faces from images.
* Learn image processing using OpenCV.
* Understand the implementation of Haar Cascade Classifiers.
* Visualize detected faces using Matplotlib.

## Technologies Used

* Python
* OpenCV (cv2)
* Glob
* Matplotlib

## Libraries Required

```python
import cv2
import glob
import matplotlib.pyplot as plt
```

## Project Workflow

### 1. Import Required Libraries

The project begins by importing the necessary Python libraries:

* **OpenCV (cv2):** Used for image processing and face detection.
* **Glob:** Used to search and retrieve image files from a directory.
* **Matplotlib:** Used for displaying images and detection results.

### 2. Load Haar Cascade Classifier

A pre-trained Haar Cascade model is loaded using:

```python
detect = cv2.CascadeClassifier('haarcascade_frontalface_default.xml')
```

This XML file contains trained data for detecting frontal human faces.

### 3. Collect Image Files

The program searches for all JPG images in the specified directory:

```python
giimage = glob.glob('/content/*.jpg')
```

The image paths are stored in a list for further processing.

### 4. Validate Image Availability

Before starting face detection, the system checks whether images are available:

* If no images are found, an error message is displayed.
* If images are available, the total number of images is printed.

### 5. Face Detection Process

For each image:

1. The image is loaded.
2. Converted to grayscale.
3. Passed through the Haar Cascade detector.
4. Faces are identified.
5. Rectangles are drawn around detected faces.

### 6. Display Results

The final output images are displayed using Matplotlib with highlighted face regions.

## Features

* Automatic image loading.
* Face detection using a pre-trained model.
* Multiple face detection support.
* Image visualization with detected faces.
* Simple and beginner-friendly implementation.

## Sample Output

The system detects faces and highlights them using rectangular bounding boxes.

Example:

```
Total images found: 5

Image 1:
Faces detected: 2

Image 2:
Faces detected: 1
```

## Applications

* Attendance Systems
* Security and Surveillance
* Facial Recognition Systems
* Human-Computer Interaction
* Smart Camera Applications


## Conclusion

This project successfully implements face detection using OpenCV's Haar Cascade Classifier. It demonstrates how machine learning-based pre-trained models can be used to identify human faces in images efficiently. The project provides a strong foundation for more advanced computer vision and facial recognition applications.

## AUTHOR 
SOURABH
