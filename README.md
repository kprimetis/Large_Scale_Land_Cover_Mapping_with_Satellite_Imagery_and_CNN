# Large-Scale Land Cover Mapping with Satellite Imagery and Convolutional Neural Networks
## Project Description
This repository contains the work for the second Project of the course "Geospatial Data Analysis" in the MSc "Data Science & Machine Learning" program. The exercise involves developing a comprehensive deep learning pipeline for land cover mapping using satellite imagery from Sentinel-2 and Convolutional Neural Networks (CNNs), specifically U-Net.

The main goals of this exercise are:

1. **Geospatial Data Acquisition and Preprocessing**: Familiarize with raster geospatial data, including pansharpening, reprojection and handling spatial references.
2. **Data Preparation for Training**: Create datasets, normalize data and apply data augmentation techniques for segmentation problems.
3. **U-Net Model Design**: Design a U-Net architecture for image segmentation, incorporating transfer learning techniques.
4. **Training and Evaluation**: Train and evaluate the U-Net model, optimize hyperparameters and monitor model performance.
5. **Prediction on New Data**: Apply the trained model to new data, create prediction maps and evaluate the results.


## Objectives
1. **Geospatial Data Acquisition and Preprocessing**

  * Download ground truth data with category names and metadata.
  * Acquire Sentinel-2 L1C products (Top-of-Atmosphere reflectance) and preprocess them (pansharpening, alignment).
  * Create image pairs of satellite data and ground truth data.

2. **Data Preparation for Training**

  * Split data into training, validation and test subsets.
  * Normalize data and apply data augmentation methods for segmentation.
  * Prepare data feeding algorithms.

3. **U-Net Model Design**

  * Design a U-Net architecture for semantic segmentation with 13 input channels and 10m spatial resolution.
  * Incorporate transfer learning using pre-trained ResNet models for the encoder part of U-Net.
  * Ensure at least two skip connections for feature transfer.

4. **Training and Evaluation**

  * Use PyTorch Lightning or similar for model training.
  * Monitor performance metrics and create relevant plots for metrics and loss functions.
  * Perform hyperparameter tuning and save the best model.

5. **Prediction on New Data**

  * Acquire Sentinel-2 L2A products (surface reflectance) and predict land cover for a different area.
  * Create prediction maps and assess the quality and quantitative metrics of the results.
