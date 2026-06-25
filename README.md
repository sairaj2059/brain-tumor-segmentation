# Brain Tumor Segmentation using U-Net

## Overview

This project implements a deep learning-based U-Net model for automatic brain tumor segmentation using multi-modal MRI scans from the BraTS 2020 dataset.

The goal is to accurately identify tumor regions from MRI images and generate pixel-wise segmentation masks that can assist in medical image analysis.

## Dataset

BraTS 2020 Training Dataset

MRI Modalities Used:

* T1
* T1CE
* T2
* FLAIR

Segmentation Labels:

* 0: Background
* 1: Necrotic / Non-enhancing Tumor Core
* 2: Peritumoral Edema
* 4: Enhancing Tumor

## Project Pipeline

1. Data Loading
2. MRI Volume Preprocessing
3. Intensity Normalization
4. Patch/Slice Extraction
5. U-Net Training
6. Segmentation Prediction
7. Performance Evaluation

## Model Architecture

U-Net Encoder-Decoder Architecture

Input:

* Multi-modal MRI images

Output:

* Pixel-wise tumor segmentation mask

Loss Functions:

* Dice Loss
* Categorical Cross-Entropy (to be finalized)

Evaluation Metrics:

* Dice Score
* IoU
* Precision
* Recall

## Current Progress

* [x] Dataset preparation
* [x] MRI visualization
* [x] Data normalization
* [x] Segmentation preprocessing
* [ ] U-Net implementation
* [ ] Model training
* [ ] Evaluation
* [ ] Inference pipeline

## Repository Structure

```text
brain-tumor-segmentation/
├── notebooks/
├── src/
├── images/
├── results/
├── README.md
├── requirements.txt
└── .gitignore
```

## Results

Training results and visualizations will be added after model development.

## Future Improvements

* Attention U-Net
* 3D U-Net
* MONAI integration
* Clinical visualization dashboard
