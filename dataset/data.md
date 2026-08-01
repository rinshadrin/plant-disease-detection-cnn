## Dataset

This project uses the **PlantVillage Dataset** (RGB images) from the `raw/color` directory.

The original PlantVillage dataset contains **38 disease and healthy leaf classes**. For this project, a **subset of 10 classes** was selected to build and evaluate the CNN model.

### Selected Classes

| Plant | Classes |
|--------|---------|
| Apple | Apple Scab, Black Rot, Healthy |
| Corn | Common Rust, Healthy |
| Grape | Black Rot, Healthy |
| Potato | Early Blight, Late Blight, Healthy |

### Dataset Source

Official Repository:
https://github.com/spMohanty/PlantVillage-Dataset

Research Paper:
https://doi.org/10.3389/fpls.2016.01419

### Dataset Preparation

1. Download the **PlantVillage Dataset**.
2. Navigate to the `raw/color` directory.
3. Use only the following **10 folders** for training:
   - Apple___Apple_scab
   - Apple___Black_rot
   - Apple___healthy
   - Corn_(maize)___Common_rust_
   - Corn_(maize)___healthy
   - Grape___Black_rot
   - Grape___healthy
   - Potato___Early_blight
   - Potato___Late_blight
   - Potato___healthy

> **Note:** The original dataset contains **38 classes**, but this project intentionally uses a **10-class subset**. The class selection is handled directly in the Jupyter Notebook during data preparation.
