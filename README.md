This repository contains scripts for classifying forested and non-forested areas using Synthetic Aperture Radar (SAR) imagery tiff files and detecting deforestation events over time.
The methods explored include both single-pixel analysis and tile-based analysis.

Directory Structure:

1 - single_pixel

**"Forest_Classification_pixel_size"** Script for classifying forest and non-forest areas using single-pixel data.
This script includes implementing Random Forest (RF) and Support Vector Machine (SVM) models, focusing on pixel-wise classification.
**"Deforestation_Event_Detection"** Script for detecting deforestation events based on the classification model trained in the single-pixel approach.
This script processes time-series SAR imagery to identify the timing of deforestation.

2 - tiles

**"Forest_Classification_pixel_size_tiles"** Script for classifying forest and non-forest areas using a tile-based approach.
This script includes implementing Random Forest (RF) and Support Vector Machine (SVM) models.
This method considers the spatial context of each pixel by analyzing a 3x3 neighborhood around each pixel, providing a more robust classification.

**"Deforestation_Event_Detection_tiles"** Script for detecting deforestation events using the tile-based classification model.
Similar to the single-pixel approach, this script processes time-series SAR imagery but leverages the enhanced spatial context from the tile-based model.

Usage:
Run Classification: Use the forest classification scripts to train and evaluate your models.
Apply the deforestation detection scripts on your time-series data to identify when deforestation events occur.
