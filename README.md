# MRI-Images-Segmentation-and-Classification

This repository contains a Jupyter notebook that focuses on **Brain MRI image analysis** using **Deep Learning**. It combines two tasks: 
1. **Segmentation** of brain tumors from MRI scans using **U-Net**.
2. **Classification** of brain MRI images (tumor / no-tumor) using CNN

## 📌 Project Overview
Medical imaging plays a vital role in diagnosing brain tumors.  
The goal of this project is to:
- Automatically **segment tumor regions** in MRI scans.
- Automatically **classify MRI scans** based on the presence of tumors.

The model is trained on the **LGG-MRI Segmentation dataset** (available on Kaggle).  



## Model Architectures

### 🔹 U-Net (Segmentation)
- Encoder (Contracting path) → extracts deep features.
- Bottleneck → compressed representation.
- Decoder (Expanding path) → reconstructs segmentation mask.
- Skip Connections → help recover fine details (like tumor boundaries).
- Output: Binary mask (`tumor = 1`, `background = 0`).

### 🔹 CNN (Classification)
- Standard CNN built on top of extracted features.
- Input: Brain MRI image.
- Output: Tumor / No-tumor (binary classification).
