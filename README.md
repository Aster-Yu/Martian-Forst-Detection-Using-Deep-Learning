# Martian Frost Detection using Deep Learning

This project classifies Martian terrain images into "frost" and "background" categories using **Convolutional Neural Networks (CNNs)** and **Transfer Learning**. The dataset is derived from NASA's HiRISE imagery, helping to study Mars' seasonal frost cycle and its climatic impacts.

---

## Project Overview

The main objectives of this project are:
- Classify Martian surface images into frost or background categories.
- Build and train a custom **CNN + MLP** model.
- Utilize **Transfer Learning** with pre-trained models like EfficientNetB0, ResNet50, and VGG16 to improve performance.
- Compare the results of custom CNNs and transfer learning approaches.

---

## Features

### 1. **Custom CNN + MLP Model**
- Built a three-layer **CNN** followed by a dense **MLP** layer.
- Techniques used:
  - **Data Augmentation**: Random crop, zoom, rotate, flip, and translation.
  - **Regularization**: Dropout (30%), Batch Normalization, and L2 Regularization.
  - Optimized with **ADAM** optimizer and **Cross-Entropy Loss**.

### 2. **Transfer Learning**
- Implemented pre-trained models:
  - **EfficientNetB0**
  - **ResNet50**
  - **VGG16**
- Fine-tuned the last fully connected layers while freezing earlier layers.
- Used extracted features for improved classification.

### 3. **Evaluation Metrics**
- Precision, Recall, and F1 Score are reported for all models.
- Training and validation losses plotted to identify model performance.

---

## Dataset

The dataset includes:
- **Images**: 299x299 tiles labeled as "frost" or "background".
- **Annotations**: JSON files containing label information for each tile.
- **Split Files**: Train, Test, and Validation splits provided.

Download the dataset from [NASA's Dataverse](https://dataverse.jpl.nasa.gov/dataset.xhtml?persistentId=doi:10.48577/jpl.QJ9PYA).
