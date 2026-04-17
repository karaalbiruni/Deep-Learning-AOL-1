# Histopathological Image Classification of Lung and Colon Cancer

This repository contains a comparative study of **EfficientNetB3** and **DenseNet121** architectures for the automated classification of lung and colon cancer histopathological images. 

## 📌 Project Overview
The accurate diagnosis of lung and colon cancer is critical for patient survival. This project implements a deep learning framework to categorize high-resolution histopathological slides into five classes. By leveraging **Transfer Learning** and **Fine-Tuning**, the system provides a robust second opinion to reduce diagnostic delays and human error in clinical settings.

## 📊 Dataset Specifications
The models were trained using the **LC25000 dataset**, which includes 25,000 color images.
* **Classes:** Colon Adenocarcinoma, Colon Benign, Lung Adenocarcinoma, Lung Squamous Cell Carcinoma, Lung Benign.
* **Preprocessing:** Images were standardized to 224x224 pixels and processed with augmentation techniques (rotation, zoom, and shifts) to ensure model generalization.

## 🚀 Model Architectures & Methodology
Two distinct deep learning strategies were evaluated:
1. **EfficientNetB3:** Optimized via compound scaling to balance depth, width, and resolution.
2. **DenseNet121:** Utilized dense connections to maximize feature reuse and gradient flow.

### Training Strategies
* **Frozen Feature Extraction:** Using pre-trained ImageNet weights to establish a baseline.
* **Selective Fine-Tuning:** Training the top layers of the architectures to adapt to the specific morphological patterns of cancerous cells.


## 🛠️ Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/karaalbiruni/Deep-Learning-AOL-1

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
