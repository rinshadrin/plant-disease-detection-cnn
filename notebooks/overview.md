## Notebook Overview

The Jupyter Notebook contains the complete workflow used to build the plant disease classification model.

The project uses RGB leaf images from the `raw/color` folder of the PlantVillage dataset. The original folder contains 38 healthy and diseased plant classes. Instead of using all 38 classes, 10 selected classes were filtered directly inside the notebook.

The notebook performs the following steps:

1. Defines the PlantVillage dataset path.
2. Reads the available class folders from the `raw/color` directory.
3. Selects 10 required classes from the original 38 classes.
4. Collects the image paths and corresponding labels.
5. Checks the number of images available in each selected class.
6. Detects corrupted or unreadable image files.
7. Checks for duplicate images in the dataset.
8. Splits the selected images into training, validation, and testing sets.
9. Preprocesses the images by resizing and normalizing them.
10. Applies data augmentation to the training images.
11. Builds a custom Convolutional Neural Network using TensorFlow and Keras.
12. Trains the model using callbacks such as Early Stopping and learning-rate reduction.
13. Evaluates the trained model using the test dataset.
14. Generates predictions for unseen leaf images.
15. Saves the trained model for future use.

## Class Selection

The complete PlantVillage `raw/color` directory contains 38 classes. The following 10 classes were selected inside the notebook:

```python
selected_classes = [
    "Apple___Apple_scab",
    "Apple___Black_rot",
    "Apple___healthy",
    "Corn_(maize)___Common_rust_",
    "Corn_(maize)___healthy",
    "Grape___Black_rot",
    "Grape___healthy",
    "Potato___Early_blight",
    "Potato___Late_blight",
    "Potato___healthy"
]
