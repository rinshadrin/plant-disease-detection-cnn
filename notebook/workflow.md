## Notebook Workflow

The Jupyter Notebook follows a complete deep learning pipeline for plant disease classification.

### 1. Dataset Preparation
- Downloaded the PlantVillage dataset (`raw/color`).
- Selected **10 classes** from the original **38 classes**.
- Loaded image paths and corresponding class labels.
- Organized the dataset for training and evaluation.

### 2. Data Inspection
- Verified the selected classes.
- Counted the number of images in each class.
- Checked for corrupted images.
- Checked for duplicate images.
- Analyzed the class distribution.

### 3. Data Preprocessing
- Resized all images to a fixed input size.
- Normalized pixel values.
- Encoded class labels.
- Split the dataset into training, validation, and testing sets.

### 4. Data Augmentation
Applied image augmentation techniques to improve model generalization, including:
- Random Flip
- Random Rotation
- Random Zoom

### 5. Model Development
Built a custom CNN architecture using TensorFlow/Keras with:
- Convolutional Layers (Conv2D)
- Batch Normalization
- MaxPooling Layers
- Global Average Pooling
- Dense Layer
- Dropout
- Softmax Output Layer

### 6. Model Training
- Compiled the model using the Adam optimizer.
- Used Sparse Categorical Crossentropy as the loss function.
- Applied Early Stopping and ReduceLROnPlateau callbacks.
- Trained the model on the prepared dataset.

### 7. Model Evaluation
- Evaluated model performance on the test dataset.
- Calculated test accuracy and loss.
- Tested the model using external images.

### 8. Results
The notebook achieved:
- **95.56% Test Accuracy**
- **96.00% External Test Accuracy**
