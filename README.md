# 🧠 Industrial Anomaly Detection with ResNet on MVTec Dataset

This project implements an image-based **anomaly detection** system using **Convolutional Neural Networks (CNNs)**, specifically **ResNet**, on the **MVTec Anomaly Detection Dataset**. It is part of the final coursework for the **Vision for Industry** class.

---

## 🧾 Project Overview

The goal is to accurately detect and classify defects in industrial product images by learning from only **normal (defect-free)** training samples. The project evaluates model performance using standard classification metrics like accuracy, confusion matrix, and ROC-AUC.

---

## 🗂️ Dataset: MVTec Anomaly Detection

- **15 industrial categories**: bottle, wood, tile, leather, screw, hazelnut, etc.
- **Training Set**: Only normal images
- **Test Set**: Includes both normal and anomalous images
- All images are resized to **224x224** and normalized

🔗 [MVTec Dataset Website](https://www.mvtec.com/company/research/datasets/mvtec-ad)

---

## 🧠 Model Architecture

- **Base Model**: Pretrained ResNet
- **Transfer Learning**: Final layers adapted for binary classification (normal vs anomaly)
- **Loss Function**: Binary Cross Entropy
- **Optimizer**: Adam
- **Epochs**: Tuned for best validation accuracy

---

## 📊 Evaluation Results

- ✅ **AUC Score**: 0.94 (Excellent distinction between normal and defective)
- ✅ **High accuracy** in categories like:
  - Leather, Wood, Carpet (1.00)
  - Hazelnut (0.98), Bottle (0.98), Tile (0.96), Zipper (0.96)
- 🔍 **Moderate to low accuracy** in categories like:
  - Toothbrush, Pill, Capsule, Screw

### 🔢 Confusion Matrix

- **True Positives**: 185  
- **True Negatives**: 698  
- **False Positives**: 28  
- **False Negatives**: 67  

---

## 📈 Key Visualizations

- ROC Curve and AUC
- Confusion Matrix
- Category-wise accuracy
- Sample predictions (correct/incorrect)

---

## 🚀 Future Work

- Use Autoencoders or GANs for unsupervised anomaly detection
- Introduce class-specific fine-tuning
- Use Grad-CAM for visual explainability of defects

---

## 👤 Author

**Ozgur Gumus**   
Vision for Industry – Final Project  
Università degli Studi di Milano, 2024

---

> This project demonstrates practical application of deep learning for industrial quality control using real-world datasets.
