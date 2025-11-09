# Deepfake-Detection-and-Media-Authentication-Agent
🔍 Description

This repository contains the implementation of a multimodal deepfake detection system designed to identify and authenticate manipulated videos, images, and audio using advanced deep learning and data science techniques.
The project integrates models like EfficientNet-B0, Vision Transformer (ViT-B/16), and LSTM to detect fake media with high accuracy and interpretability.

📘 Introduction

With the rise of AI-generated media (deepfakes), ensuring the authenticity of digital content has become a global challenge. Deepfakes can manipulate human faces, voices, and actions, posing severe threats to privacy, journalism, and digital trust.

This project aims to develop a reliable AI system that detects such manipulations across multiple formats—video, image, and audio—while maintaining explainability and scalability.
By combining the power of computer vision, natural language processing, and data science, the system delivers accurate predictions and visual justifications using Grad-CAM heatmaps.

⚙️ Methodology Overview

The system follows a modular data science pipeline:

Data Collection

Video Dataset: FaceForensics++ (C23)

Image Dataset: Hard Fake vs Real Faces

Audio Dataset: FakeAVCeleb (Extracted Audio)

Data Preprocessing

Frame extraction from videos (1–2 FPS)

Image resizing (224×224) and normalization

Audio converted into log-mel spectrograms

Augmentations: flipping, noise, brightness changes

Model Development

EfficientNet-B0 → Frame-level video analysis

ViT-B/16 → Image manipulation detection

LSTM → Audio spectrogram classification

Training

Transfer learning & fine-tuning

3-fold cross-validation

Loss: Binary Cross-Entropy | Optimizer: Adam

Evaluation

Metrics: Accuracy, Precision, Recall, F1-score, AUC-ROC

Visualization: Grad-CAM heatmaps & ROC curves
