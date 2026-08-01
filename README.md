# 🌿 Plant Disease Detection and Classification Using CNN

A deep learning project that detects and classifies plant leaf diseases using a **Convolutional Neural Network (CNN)** built with **TensorFlow** and **Keras**.

## Overview

This project trains a CNN model on a subset of the **PlantVillage** dataset to classify healthy and diseased plant leaves. The workflow covers data preprocessing, image augmentation, model training, evaluation, and prediction.

### Dataset

- **Dataset:** PlantVillage (RGB Images)
- **Total Images:** 9,005
- **Classes:** 10

### Disease Classes

| Plant | Classes |
|--------|---------|
| Apple | Apple Scab, Black Rot, Healthy |
| Corn | Common Rust, Healthy |
| Grape | Black Rot, Healthy |
| Potato | Early Blight, Late Blight, Healthy |

---

## Results

| Metric | Value |
|--------|------:|
| Training Images | 6,303 |
| Validation Images | 1,351 |
| Testing Images | 1,351 |
| Test Accuracy | **95.56%** |
| External Test Accuracy | **96.00%** |

> Results are based on the saved notebook execution. Accuracy may vary slightly when the model is retrained.

---

## Model Architecture

- Image Augmentation
- Conv2D Layers
- Batch Normalization
- Max Pooling
- Global Average Pooling
- Dense Layer
- Dropout
- Softmax Output
- Adam Optimizer
- Early Stopping

---

## Repository Structure

```text
plant-disease-detection-cnn/
│
├── dataset
├── models/
├── notebooks/
│   └── plant_disease_cnn.ipynb
│   └── overview.md
│   └── workflow.md
│
├── README.md
└── .gitignore
```

---

## Installation

Clone the repository:

```bash
git clone https://github.com/YOUR_USERNAME/plant-disease-detection-cnn.git
cd plant-disease-detection-cnn
```

Create a virtual environment (optional):

```bash
python -m venv .venv
```

Activate it:

**Windows**

```bash
.venv\Scripts\activate
```

**Linux/macOS**

```bash
source .venv/bin/activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

## Download Dataset

```bash
git clone https://github.com/spMohanty/PlantVillage-Dataset.git data/PlantVillage-Dataset
```

Expected dataset path:

```
data/
    PlantVillage-Dataset/
        raw/
            color/
```

Run the notebook:

```bash
jupyter notebook notebooks/plant_disease_cnn.ipynb
```

---

## Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Pandas
- Matplotlib
- Pillow
- Scikit-learn
- Jupyter Notebook

---

## Dataset Source

**PlantVillage Dataset**

Official Repository:
https://github.com/spMohanty/PlantVillage-Dataset

Research Paper:

Mohanty, S. P., Hughes, D. P., & Salathé, M. (2016).

*Using Deep Learning for Image-Based Plant Disease Detection.*

https://doi.org/10.3389/fpls.2016.01419

---

## Limitations

The PlantVillage dataset contains images captured under controlled conditions. Model performance may differ on real-world field images due to varying lighting, backgrounds, camera angles, and disease stages.

---

## Author

**Muhammed Rinshad**

Data Science & AI

GitHub: https://github.com/rinshadrin

---
