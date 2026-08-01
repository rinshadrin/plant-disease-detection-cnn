# 🌿 Plant Disease Detection and Classification Using CNN

![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange.svg)
![Keras](https://img.shields.io/badge/Keras-Deep%20Learning-red.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)
![Status](https://img.shields.io/badge/Project-Completed-success.svg)

A deep learning-based image classification system that automatically detects and classifies plant leaf diseases using a custom **Convolutional Neural Network (CNN)** built with **TensorFlow** and **Keras**.

The model is trained on a curated subset of the **PlantVillage Dataset** containing RGB images of healthy and diseased leaves from multiple crop species. The project demonstrates the complete deep learning workflow, including data preprocessing, exploratory analysis, augmentation, model training, evaluation, and prediction.

---

# 📌 Table of Contents

- Project Overview
- Features
- Dataset
- Disease Classes
- Model Pipeline
- Project Structure
- Results
- Installation
- Usage
- Model Architecture
- Future Improvements
- Limitations
- Technologies Used
- References
- Author
- License

---

# 📖 Project Overview

Early detection of plant diseases plays a crucial role in reducing crop loss and improving agricultural productivity.

This project develops a CNN-based image classification model capable of identifying **10 different classes** of healthy and diseased plant leaves with high accuracy.

The project includes:

- Dataset inspection
- Image quality verification
- Corrupted image detection
- Duplicate image checking
- Class distribution analysis
- Image preprocessing
- Data augmentation
- Stratified Train/Validation/Test split
- CNN model development
- Model evaluation
- Prediction on unseen images
- Performance visualization

---

# ✨ Features

- Custom CNN architecture
- TensorFlow & Keras implementation
- Data augmentation
- Batch Normalization
- Dropout regularization
- Early Stopping
- Learning Rate Scheduler
- Duplicate image detection
- Corrupted image filtering
- Training history visualization
- Confusion Matrix
- Classification metrics
- External image testing

---

# 🌱 Dataset

This project uses the **PlantVillage Dataset**.

### Dataset Statistics

| Item | Value |
|------|-------|
| Images Used | **9,005** |
| Classes | **10** |
| Image Type | RGB |
| Source | PlantVillage |

The dataset is **not included** in this repository due to its size.

## Dataset Sources

### Official GitHub

https://github.com/spMohanty/PlantVillage-Dataset

### TensorFlow Dataset

https://www.tensorflow.org/datasets/catalog/plant_village

### Research Paper

Mohanty, Hughes & Salathé (2016)

**Using Deep Learning for Image-Based Plant Disease Detection**

https://doi.org/10.3389/fpls.2016.01419

---

# 🍃 Disease Classes

| Plant | Disease |
|--------|----------|
| Apple | Apple Scab |
| Apple | Black Rot |
| Apple | Healthy |
| Corn | Common Rust |
| Corn | Healthy |
| Grape | Black Rot |
| Grape | Healthy |
| Potato | Early Blight |
| Potato | Late Blight |
| Potato | Healthy |

---

# ⚙️ Project Pipeline

```
Dataset Collection
        │
        ▼
Dataset Inspection
        │
        ▼
Corrupted Image Check
        │
        ▼
Duplicate Image Detection
        │
        ▼
Data Preprocessing
        │
        ▼
Image Augmentation
        │
        ▼
Train / Validation / Test Split
        │
        ▼
CNN Model Training
        │
        ▼
Model Evaluation
        │
        ▼
Prediction on New Images
```

---

# 📂 Repository Structure

```
plant-disease-detection-cnn/
│
├── data/
│   └── README.md
│
├── models/
│   └── .gitkeep
│
├── notebooks/
│   └── plant_disease_cnn.ipynb
│
├── requirements.txt
├── README.md
├── DATASET.md
├── CITATION.cff
├── LICENSE
└── .gitignore
```

---

# 📊 Results

| Evaluation | Result |
|------------|--------|
| Total Images | 9,005 |
| Training Images | 6,303 |
| Validation Images | 1,351 |
| Testing Images | 1,351 |
| Test Accuracy | **95.56%** |
| External Test Accuracy | **96.00%** |

> Results shown above are obtained from the saved notebook execution. Accuracy may vary slightly depending on hardware, TensorFlow version, random initialization, and retraining.

---

# 🚀 Installation

## Clone Repository

```bash
git clone https://github.com/rinshadrin/plant-disease-detection-cnn.git
cd plant-disease-detection-cnn
```

---

## Create Virtual Environment

### Windows

```bash
python -m venv .venv

.venv\Scripts\activate
```

### macOS / Linux

```bash
python3 -m venv .venv

source .venv/bin/activate
```

---

## Install Dependencies

```bash
pip install -r requirements.txt
```

---

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

---

## Run Notebook

```bash
jupyter notebook notebooks/plant_disease_cnn.ipynb
```

Run Jupyter from the repository root so that all relative paths resolve correctly.

---

# 🧠 Model Architecture

The CNN architecture consists of:

- Image Augmentation Layer
- Conv2D
- Batch Normalization
- MaxPooling
- Conv2D
- Batch Normalization
- MaxPooling
- Conv2D
- Batch Normalization
- MaxPooling
- Global Average Pooling
- Dense Layer
- Dropout
- Softmax Output Layer

Training configuration:

- Optimizer: Adam
- Loss Function: Sparse Categorical Crossentropy
- Activation: ReLU
- Output Activation: Softmax
- Early Stopping
- ReduceLROnPlateau

---

# 🔮 Future Improvements

- MobileNetV3 implementation
- EfficientNet implementation
- Transfer Learning
- Grad-CAM visualization
- Streamlit Web Application
- Flask REST API
- ONNX model export
- TensorFlow Lite deployment
- Real-time camera prediction
- Multi-label disease detection

---

# ⚠️ Limitations

The PlantVillage dataset contains images captured under controlled laboratory conditions with relatively clean backgrounds.

Although the model achieves high accuracy on this dataset, real-world agricultural environments involve varying lighting conditions, complex backgrounds, camera angles, and disease stages.

Further evaluation using field-collected images is recommended before practical deployment.

---

# 🛠 Technologies Used

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

# 📚 References

Mohanty, S. P., Hughes, D. P., & Salathé, M.

Using Deep Learning for Image-Based Plant Disease Detection

Frontiers in Plant Science (2016)

https://doi.org/10.3389/fpls.2016.01419

---

# 👨‍💻 Author

**Muhammed Rinshad**

Data Science & AI

GitHub: https://github.com/YOUR_USERNAME

LinkedIn: https://linkedin.com/in/YOUR_LINKEDIN

---

# 📄 License

This project is licensed under the **MIT License**.

The PlantVillage Dataset is distributed under its own licensing terms and is **not covered** by the MIT License included in this repository.
