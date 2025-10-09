
# Turkiye Detect — Rubble Detection Training & Inference
This repository provides a pair of preset notebooks that demonstrate how to **train** and **run inference** for rapid rubble detection from satellite imagery in the aftermath of an earthquake. It is part of a broader effort to design effective deep learning models for geospatial applications.

## Contents

### (A) `Turkey Detect Model training.ipynb`
Trains a **Mask R-CNN** model with **Detectron2** on a custom dataset of 1024×1024 image tiles.
- Dataset: tiles from satellite imagery with **train/val/test** splits.
- Annotations: **COCO-style** labels created with **CVAT**.
- Notebook covers: data setup, model configuration, training, and evaluation.

### (B) `Turkiye Detect Inference Runner.ipynb`
Runs inference on new imagery using a trained model.
- Loads the saved configuration and weights, builds a Detectron2 predictor.
- Accepts a **GeoTIFF (`.tif`)** scene, automatically tiles it, and runs inference.
- Exports a **Shapefile (`.shp`)** of the predictions and a rendered image with the inference overlays.


### (C) 'WebMaps'
Generate simple webmaps with the resulting .shp

