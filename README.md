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
├── results/
├── README.md
├── requirements.txt
└── .gitignore
```

## Development Environment

This project is being developed and executed using Kaggle Notebooks.

The code, preprocessing pipeline, model training, and evaluation are designed to run directly within the Kaggle environment using the BraTS 2020 dataset available through Kaggle Datasets.

## Running the Project

### Option 1: Run on Kaggle (Recommended)

1. Open the project notebook(s) in Kaggle.
2. Attach the BraTS 2020 dataset to the notebook.
3. Enable GPU acceleration from:

   * Settings → Accelerator → GPU
4. Run all cells sequentially.

### Option 2: Run Locally

The project can also be adapted for local execution by:

1. Downloading the BraTS 2020 dataset.
2. Updating dataset paths in the notebook or source code.
3. Installing dependencies listed in `requirements.txt`.
4. Running the preprocessing and training notebooks/scripts.

## Notes

* Development and experimentation are performed on Kaggle.
* Dataset files are not included in this repository because of their large size.
* Model checkpoints and generated outputs are excluded from version control.
* Progress, results, and improvements will be updated as the project evolves.


## Results

Training results and visualizations will be added after model development.

## Future Improvements

* Attention U-Net
* 3D U-Net
* MONAI integration
* Clinical visualization dashboard
