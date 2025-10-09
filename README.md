# Turkiye Detect

This repository contains few preset codes that showcase the training of a deep learning model for rapid rubble detection from satellite imagery in the aftermath of an earthquake. 
This is part of a project to design effective deep learning models for geospatial applications. 

The Repository contains the following files:

(A) Turkey Detect Model training.ipynb

This code shows the training of a maskrCNN model using detectron2 library on a custom dataset. The dataset is composed of 1024x1024 tiles that make up a portion of the satellite image, these tiles are split in train, test, val. The dataset includes COCO-Style annotations made with CVAT.ai. 

The code thus trains the model, runs model evaluation.

(B) Turkiye Detect Inference Runner .ipynb

This code is used to run inference on different available images of the scene; the model configuration and weights are loaded and a predictor is assembled. Then, the model is fed a .tif image, the model tiles it, runs inference and exports the .shp alongside an image of the inference. 

![System diagram](Screenshot 2025-10-09 at 18.41.17.png)
