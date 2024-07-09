# Sienna

# Overview
This project implements a convolutional neural network (CNN) classifier to identify diseases in leaf images. The CNN is trained to classify images into three categories: Angular Leaf Spot, Bean Rust, and Healthy leaves. The model architecture used here is MobileNetV2 due to its efficiency and effectiveness in mobile and embedded vision applications.

# Preprocessing Steps
The input leaf images undergo several preprocessing steps before being fed into the CNN for classification. These steps include:

  1. Color Domain Conversion: Converting the images to a suitable color space (e.g., RGB to HSV) for better feature extraction.

  2. Histogram Equalization: Improving the contrast and brightness of the images to enhance feature visibility.

  3. Noise Removal: Applying filters (e.g., Gaussian blur) to reduce noise and smoothen the images.

  4. Contour Detection: Utilizing the Canny Edge detector to detect edges and contours, which helps in delineating the leaf structure from the background.

# Model Architecture
The CNN model architecture chosen for this project is MobileNetV2. MobileNetV2 is selected due to its lightweight nature, making it suitable for deployment on mobile devices and embedded systems without compromising much on accuracy.

# Training Details
  1. Dataset: The model is trained on a dataset consisting of annotated leaf images across the three categories.

  2. Training Procedure: The MobileNetV2 model is trained using transfer learning. Specifically, the pre-trained MobileNetV2 model is fine-tuned on the leaf dataset to adapt to the specific classification task.

  3. Training Parameters: The model is trained using stochastic gradient descent (SGD) with a learning rate scheduler and momentum optimization.

# Evaluation Metrics
The performance of the classifier is evaluated using standard metrics such as accuracy, precision, recall, and F1-score. These metrics provide insights into how well the model performs across different classes.
