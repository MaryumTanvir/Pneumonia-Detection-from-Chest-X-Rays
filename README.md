
# Pneumonia Detection from Chest X-Rays

---

##  Overview

This project implements a deep learning-based approach to detect **Pneumonia** in **chest X-ray images** using convolutional neural networks (CNNs). The primary goal is to assist radiologists by automating the classification of X-rays into:

- **NORMAL**
- **PNEUMONIA**

---

##  Dataset

- **Name:** Chest X-Ray Images (Pneumonia)  
- **Source:** [Kaggle Dataset by Kermany et al.](https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia)  
- **Description:** Contains over 5,000 labeled X-ray images categorized into **train**, **test**, and **val** directories.

---

##  Tasks Performed

### 1.  Dataset Exploration

- Loaded and visualized sample images.
- Analyzed class distribution and imbalance.

### 2.  Data Preprocessing

- Resized images to a consistent input size.
- Normalized pixel values to improve training.
- Applied **image augmentation** (rotation, zoom, shift, flip) to address class imbalance and improve generalization.

### 3.  Model Development

Two model approaches were implemented:

####  CNN Model from Scratch

- Built a custom CNN architecture using Conv2D, MaxPooling, Dropout, and BatchNormalization layers.

####  Transfer Learning (ResNet)

- Leveraged pretrained model with fine tuning for improved performance on medical imaging.

### 4.  Model Evaluation

- Evaluated using:
  - Accuracy
  - Precision, Recall, F1-score
  - Confusion Matrix
- Plotted training and validation accuracy/loss curves.

---

##  How to Run

1. Clone the repository or open the `.ipynb` file in Jupyter Notebook / Google Colab.
2. Ensure dataset is placed in the expected directory structure (`chest_xray/train`, `test`, `val`).
3. Run each cell step by step.
4. Outputs such as metrics, plots, and Grad-CAM heatmaps will be generated inline.

---

##  Challenges & Lessons

- Managing dataset imbalance was key to improving recall.
- Data augmentation greatly helped model generalization.
- Grad-CAM provided useful insights into model trustworthiness.

---
```

