# MRI-Images-Segmentation-and-Classification

This repository contains a Jupyter notebook that focuses on **Brain MRI image analysis** using **Deep Learning**. It combines two tasks: 
1. **Segmentation** of brain tumors from MRI scans.
2. **Classification** of brain MRI images (tumor / no-tumor).

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

### 🔹 Pretrained ResNet50 (Classification)
- Input: Brain MRI image.
- Output: Tumor / No-tumor (binary classification).

## Plots of Segmentation

<img width="500" height="500" alt="Screenshot 2025-08-18 151314" src="https://github.com/user-attachments/assets/4fe83d40-087e-4bb5-af30-2ba3002fc1a1" />
<img width="500" height="500" alt="Screenshot 2025-08-18 151414" src="https://github.com/user-attachments/assets/90b38203-c47b-49b0-8fd6-54ff550a530e" />



