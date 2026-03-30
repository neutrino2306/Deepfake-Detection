# Deepfake Detection System

This repository contains my undergraduate research project on deepfake detection, where I built an end-to-end system covering model development, backend services, and a lightweight frontend for interactive testing.

## Overview

The project consists of three main components:

- **Modeling:** Design and training of deep learning models for deepfake detection  
- **Backend:** Data preprocessing, training pipelines, and inference services  
- **Frontend:** Simple interface for visualizing detection results and testing model outputs  

The goal of this project was to explore robust feature representations for deepfake detection and improve generalization across different datasets.

## Model Development

I experimented with multiple model architectures and training strategies throughout the project.

- Started with XceptionNet-based models for spatial feature extraction  
- Incorporated CBAM (attention mechanisms) to enhance feature representation  
- Explored different data preprocessing pipelines and training configurations  
- Iterated across multiple model variants to improve robustness  

Through these experiments, I observed that models relying solely on spatial features often struggled with cross-domain generalization.

## Final Architecture

To address this, I designed a **dual-branch model**:

- **Spatial branch:** EfficientNet-B4  
- **Frequency branch:** Frequency-domain features (e.g., FFT, DCT)  

By combining spatial and frequency-domain information, the model was able to capture complementary signals and improve robustness to unseen data.

## Design Considerations

During development, I had to balance:

- Model complexity vs. generalization performance  
- Training cost vs. performance gains  
- Iteration speed vs. architectural exploration  

Introducing frequency-domain features improved robustness, but also increased model complexity and training time. I iterated across different designs to find a practical balance that could be trained efficiently while still achieving strong performance.

## Repository Structure

- `backend/` – Backend services for data handling and model inference  
- `frontend/` – Frontend interface for testing and visualization  
- `models/`
  - `data_preprocess/` – Data preprocessing pipelines and scripts  
  - `models/` – Model architectures and experimental variants  
  - `train/` – Training scripts and configurations  
  - `test/` – Evaluation and testing scripts  

## Notes

This repository reflects an experimental research process, including multiple model iterations and exploratory implementations.
