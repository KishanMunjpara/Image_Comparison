# Image Difference Detection

This project implements image difference detection using both traditional computer vision techniques with OpenCV and a deep learning approach with scikit-image. The goal is to identify differences between two images, draw bounding boxes around varying regions, and calculate a similarity score.

# DEMO
1. DEMO : (https://graphical-contrast-evaluation.onrender.com)
   
## Table of Contents

- [Introduction](#1-introduction)
- [Methodology](#2-methodology)
  - [Traditional Computer Vision Approach](#21-traditional-computer-vision-approach)
  - [Deep Learning Approach with scikit-image](#22-deep-learning-approach-with-scikit-image)
- [Results](#4-results)


## 1. Introduction

The objective of this project is to develop a computer vision model capable of identifying differences between two images, drawing bounding boxes around varying regions, and calculating a similarity score. The comparison is implemented using both traditional computer vision techniques and deep learning models.

## 2. Methodology

### 2.1 Traditional Computer Vision Approach

The traditional computer vision approach involves the following steps:
- Read and resize two input images.
- Convert the images to grayscale.
- Compute the absolute difference between the grayscale images.
- Apply thresholding to create a binary difference mask.
- Utilize morphological operations (dilation) to enhance the differences.
- Identify contours and draw bounding boxes around significant differences.

### 2.2 Deep Learning Approach with scikit-image

The deep learning approach uses the structural similarity index (SSIM) for image comparison:
- Read and resize two input images.
- Convert the images to grayscale.
- Calculate the SSIM between the two images.
- Create a difference mask based on the SSIM values.
- Apply thresholding to obtain a binary difference mask.
- Identify contours and draw bounding boxes around significant differences.
- Display the SSIM value on one of the images.

## 4. Results
1. Traditional Computer Vision Approach : ![Traditional Computer Vision Approach](https://drive.google.com/uc?id=1pHJthQbnizDCHZKWthrB7cyqxv3EBgGO)
2. Deep Learning Approach with scikit-image : ![Deep Learning Approach with scikit-image](https://drive.google.com/uc?id=13Nb2juqVm6y_giHbBvcJ7kkM5oA7XNRR)

## License
This project is licensed under the [MIT] License - see the [LICENSE](LICENSE) file for details.
