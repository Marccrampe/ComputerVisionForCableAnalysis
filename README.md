### Repository Name: Computer Vision for Cable Analysis

## Description:
This repository contains a project focused on using computer vision techniques to automate the analysis of cable images. The project aims to streamline the process of identifying and counting cables in images, which is crucial for infrastructure management and inspection tasks.

## Features:
- **Image Preprocessing**: Isolates and enhances features representing cables, specifically targeting bright cyan blue colors.
- **Cable Categorization**: Utilizes a Convolutional Neural Network (CNN) to classify the types of cables (e.g., 'F-Duct', 'Dac', 'Other').
- **Cable Counting**: Segments images and applies image processing techniques to accurately count the number of cables present.
- **Automated Workflow**: Combines preprocessing, categorization, and counting into a seamless, automated pipeline.

## Workflow Overview:
1. **Preprocessing**:
    - The images are preprocessed to filter out all colors except bright cyan blue, isolating the cables.
    - This is achieved using color space conversion and masking techniques in OpenCV.

2. **Cable Categorization using CNN**:
    - A Convolutional Neural Network (CNN) model is employed to classify the types of cables in the images.
    - The CNN architecture includes multiple convolutional layers, pooling layers, and fully connected layers, which are trained to identify and differentiate between different types of cables.
    - The model is trained on labeled images and achieves a high level of accuracy in classifying cable types.

3. **Cable Counting using Slicing Method**:
    - The images are sliced into vertical or horizontal sections to simplify the counting process.
    - Each slice is processed to identify and count the cables within it.
    - Adaptive thresholding and contour detection techniques are used to accurately count the cables in each slice.
    - The slicing method provides a detailed count and helps in dealing with images where cables might overlap or be in close proximity.

## Usage:
1. **Preprocess Images**:
    - The `preprocess_image` function filters images to isolate cables based on color characteristics.
2. **Classify Cables**:
    - The `identify_cable_type` function uses the CNN model to categorize the type of cables in the images.
3. **Count Cables**:
    - The `slice_and_count_wires` function slices images and counts the number of cables detected in each slice.



## Credits:
This project was developed by [Marc Crampe](https://www.linkedin.com/in/marc-crampe-bb80b1258/) as part of the Inframent initiative.

Feel free to modify the description and example code to better fit your project specifics and needs.
