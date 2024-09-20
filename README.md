# SAM-Sentinel-Water

This repository contains code that adapts Meta AI's Segment Anything Model (SAM) to work with satellite images for monitoring water reservoirs. The model is fine-tuned to predict water areas, helping to track changes in water levels over time using satellite imagery.

## Project overview

Water resource monitoring is crucial for understanding environmental changes and managing water supply. This project uses the SAM model, designed for segmentation tasks, and applies it to Sentinel satellite images. The images were first pre-processed and download on Google Earth Engine (see below). The input is composed of a collection of four 3-bands images, each one representing the median of a season (e.g. JJA). A further processing is include in the provided code. 
### Features:
- Adapts SAM for segmentation of water bodies in Sentinel images
- Utilizes satellite imagery to monitor water levels in reservoirs
- Enables predictions from user clicks (interactive segmentation) or fixed clicks
- Includes code to process and visualize results in Google Colab

The results are presented in the form of:
- Accuracy metrics
- Visualization of the confusion matrix
- Maps of the F1 score basing on the location of the click

## Additional resources

[Google Earth Engine code to download images](https://code.earthengine.google.com/8ddb0fcce9dd531e811015b1bcf673e3)
