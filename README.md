# NYCU Computer Vision 2025 Spring HW3
StudentID:110550142  
Name:黃芷柔  

## Introduction
Instance segmentation in biomedical images is a critical task, especially for analyzing cell morphology, distribution, and classification. Accurate segmentation of individual cells enables downstream tasks such as cell counting, phenotype analysis, and disease diagnosis.  
To tackle this problem, we adopt Mask R-CNN with a ResNet-50 backbone and FPN (Feature Pyramid Network). Mask R-CNN is a well-established framework for instance segmentation, combining object detection and pixel-wise mask prediction. The FPN backbone enhances feature extraction across multiple scales, which is particularly important for capturing both small and large cells. 
In this project, we aim to improve the performance of the base Mask R-CNN model on a given cell segmentation dataset. Our goal is to maximize detection accuracy while maintaining model compactness and generalization ability.  




## How to install
You can run this project directly in your browser using Google Colab. No local setup is needed.

Steps:
Click the badge above to open the notebook in Google Colab.  

Run all cells in the notebook to install dependencies, train, and evaluate the model.  

📦 All required packages will be installed automatically in the notebook.  

⚠️ Make sure you are using a GPU runtime by going to

   `Runtime > Change runtime type > Hardware accelerator > GPU`




## Performance snapshot

```
AP50    0.3666  (public)/ 0.3962 (private)
Backbone	Mask R-CNN with MobileNetV3-FPN  
Training Epochs	5
Dataset	Raw .tif images with 4-class instance masks. Preprocessed to uniform resolution before training. 188 training, 21 validation samples.
