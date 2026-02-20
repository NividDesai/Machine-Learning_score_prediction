# Image Classification & Segmentation Project

This folder contains advanced computer vision workflows focused on defect detection and localization in industrial manufacturing, specifically using the MVTec metal nut dataset.

## Folder Overview
The `Image classification` folder explores both supervised and unsupervised approaches to maintaining quality control in a production environment. It demonstrates how different machine learning paradigms—from classical clustering to modern deep learning—can be applied to the same problem set.

## Files Description

### 1. `CNN_Defect_Segmentation.ipynb`
This notebook implements a state-of-the-art **Semantic Segmentation** pipeline using the **U-Net architecture**.
- **Objective**: Move beyond simple "defect detection" to "defect localization" by generating pixel-level masks.
- **Workflow**:
  - **Data Handling**: Loads industrial images and their corresponding binary ground-truth masks.
  - **Architecture**: Employs a Convolutional Neural Network (CNN) in a U-Net configuration (encoder-decoder with skip connections).
  - **Results**: Successfully highlights physical damages such as scratches, discolorations, and structural deformations (bent/flipped nuts).
  - **Impact**: Provides a tool for automated visual inspection that shows operators exactly where a part is failing quality standards.

### 2. `Unsupervised_Learning_Clustering.ipynb`
This notebook explores **Anomaly Detection** through the lens of unsupervised learning.
- **Objective**: Identify defective parts without requiring labeled training data for every defect type.
- **Workflow**:
  - **Feature Extraction**: Uses a pretrained **VGG16** model (Transfer Learning) to convert images into high-dimensional feature vectors.
  - **Dimensionality Reduction**: Applies **Principal Component Analysis (PCA)** to simplify features while preserving variance.
  - **Clustering Algorithms**: Compares **K-means** (centroid-based) and **DBSCAN** (density-based) for separating "good" samples from anomalies.
  - **Visualization**: Utilizes **t-SNE** to map high-dimensional clusters into 2D space, visually demonstrating how defects naturally separate from standard parts.
- **Findings**: Evaluates which clustering metrics (Silhouette, Elbow method) best capture industrial anomalies.

## Learning Path
1. **Unsupervised Approach**: Start with `Unsupervised_Learning_Clustering.ipynb` to understand how raw image features group together naturally.
2. **Supervised Approach**: Follow up with `CNN_Defect_Segmentation.ipynb` to see how target labels and deep learning can achieve precise localization of identified defects.
