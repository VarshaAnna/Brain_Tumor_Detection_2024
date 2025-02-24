# Pixel-Based Brain Tumor Detection Using MRI Scans
Capstone Project | University of North Carolina at Greensboro | Aug 2023 – Dec 2024

### Abstract

**Pixel Based Machine Learning technique manages each pixel as a data point from a Magnetic Resonance Image (MRI) scan for analysis and classification. Considering the Brain Tumor detection application, it is important that we identify details and analyze each pixel in isolation to pinpoint every minute and irregularly shaped affected region of the brain. As a result, to build such a machine learning model, in reality we have a need for significant amount of data of multiple subjects, ensuring precision and generalization. However, Pixel
Based Brain Tumor Detection with MRI data of multiple subjects can be a root of significant discrepancies in special context and is susceptible to noise due to the heterogeneity of
brain structures and tumor characteristics. And hence to handle such complications we need Machine Learning Technique that is trained in such an environment.**

**In this paper, we utilized the image filtering-based feature extraction techniques using 10 image filters alongside a pixelbased brain tumor detection technique where the model is trained using Random Forest classifier on multiple subjects so that it can predict tumor independent to brain structure.**
--------------------------------------------------------------------------------------------------

**Project Overview**

Brain tumors are among the most critical neurological conditions requiring precise detection and classification. This project focuses on pixel-based brain tumor detection using MRI scans from the BraTS 2020 dataset., leveraging advanced image processing techniques and machine learning models to improve tumor segmentation and classification.

**Key Features**

- Dataset: Utilized BraTS 2020 MRI dataset (T2-FLAIR modality).
- Feature Engineering: Applied 14 image processing filters to extract pixel-based features.
- Machine Learning Model: Implemented a Random Forest classifier for tumor classification.
- Dataset Balancing: Used random sampling to balance tumor and non-tumor samples.
- Model Evaluation: Compared 8-feature and 14-feature feature spaces for performance.
- Visualization: Plotted ROC curves, feature importance, and classification results.

**Dataset & Preprocessing**

The dataset consists of volumetric MRI scans, processed as follows:
- Segmentation Extraction: Isolated enhancing tumor regions from segmentation masks.
  ![Enhancing Tumor, 4th Lable]<img src="https://github.com/VarshaAnna/Brain_Tumor_Detection_2024/blob/main/Final%20report%20images/label4.PNG?raw=true">
  
- Feature Space Construction: Extracted 14 image features for tumor detection.
  <img src="https://github.com/VarshaAnna/Brain_Tumor_Detection_2024/blob/main/Final%20report%20images/Image%20processing%20tech..png?raw=true" width="500">
  
  <img src="https://github.com/VarshaAnna/Brain_Tumor_Detection_2024/blob/main/Final%20report%20images/Feature%20space%20construction.png?raw=true" width="500">
  
- Balanced Feature Space: Matched tumor and non-tumor sample sizes to prevent bias.
  ![Balancing Feature Space]<img src="https://github.com/VarshaAnna/Brain_Tumor_Detection_2024/blob/main/Final%20report%20images/Balancing%20dataset.png?raw=true" width="500">

**Image Processing Filters Used**

Here are the 14 filters applied for feature extraction:
- Gaussian blurring
- Canny edge detection
- Sobel x operator
- Sobel y operator
- Laplacian filtering
- Histogram of Oriented Gradients (HOG)
- Gradient magnitude
- Gradient direction
- Median filter
- Bilateral filter

<img src="https://github.com/VarshaAnna/Brain_Tumor_Detection_2024/blob/main/Final%20report%20images/Image%20processing%20Filters.png?raw=true" width="500">

**Methodology**

<img src="https://github.com/VarshaAnna/Brain_Tumor_Detection_2024/blob/main/Final%20report%20images/Brain%20tumor%20detection%20flowchart%20(1).png?raw=true" width="500">

**Model Performance**

We evaluated the performance of the Random Forest classifier on multiple volumetric datasets.

**Conclusion**

- The 8-feature space surprisingly outperformed the 14-feature space, possibly due to noise introduced by additional features.
- The Random Forest model demonstrated strong generalization across multiple volumetric datasets.
- Future work includes testing with deep learning models and further feature selection techniques to refine tumor classification.
