# 🔍 Industrial Anomaly Detection with CNNs on MVTec Dataset

This project applies a **Convolutional Neural Network (CNN)** based approach, using **ResNet**, to detect visual anomalies in industrial inspection tasks. Using the **MVTec Anomaly Detection Dataset**, the goal is to classify images of objects as either normal or defective.

---

## 📦 Dataset: MVTec Anomaly Detection

The MVTec dataset consists of **15 object categories** commonly found in industrial applications. Each category contains:

- ✅ **Training Set**: Only normal (non-defective) images
- 🚨 **Test Set**: Both normal and anomalous images
- All images are resized to `224x224` and normalized during preprocessing.

Example categories: `bottle`, `hazelnut`, `wood`, `tile`, `carpet`, `leather`, `screw`, `pill`, etc.

🔗 [Official Dataset Site](https://www.mvtec.com/company/research/datasets/mvtec-ad)

---

## 🧠 Why ResNet?

- **Deeper architecture** enables learning of complex patterns
- **Residual connections** solve vanishing gradient issues
- Proven **high performance in image classification tasks**

---

## 🧪 Methodology

1. **Data Preprocessing**:
   - Resize images to 224x224
   - Normalize pixel values

2. **Model Architecture**:
   - Based on pretrained **ResNet**
   - Custom classification head

3. **Training Strategy**:
   - Trained on normal samples only
   - Evaluated on normal + defective images
   - Evaluated using Accuracy, Confusion Matrix, ROC-AUC

---

## 📈 Results

- **AUC Score**: `0.94`
- **High-performing categories**: Leather, Wood, Carpet, Hazelnut, Bottle
- **Moderate performance**: Tile, Transistor, Toothbrush
- **Low performance**: Capsule, Screw

### Confusion Matrix

- True Positives: `185`
- True Negatives: `698`
- False Positives: `28`
- False Negatives: `67`

---

## 🎥 Demo & Visuals

Check the Jupyter Notebook for:
- NDVI visualizations
- ROC curve
- Model predictions (correctly & incorrectly classified)

---

## 📊 Project Files

| File | Description |
|------|-------------|
| `VisionFinal.ipynb` | Notebook with full model, training, and evaluation |
| `Project.pptx` | Final project presentation |

---

## 🧠 Future Improvements

- Introduce **autoencoders** or **GAN-based anomaly detection**
- Fine-tune the model per category
- Use **attention-based mechanisms** to improve weak-performing classes

---

## 👥 Authors

- **Ozgur GUmus** (910427)

---

