# 🏆 Sports Image Classification using Deep Learning (Custom CNN & MobileNetV2)

## 📌 Project Overview

This project develops a deep learning framework for **multi-class sports image classification** using Convolutional Neural Networks (CNNs). The objective is to automatically classify sports images into one of **100 different sports categories**.

The project compares a **Custom CNN** with **MobileNetV2** (Transfer Learning) and evaluates their performance using multiple classification metrics and Explainable AI techniques such as **Grad-CAM**.

---

# 📖 Dataset

**Dataset Name:** Sports Image Classification

- **Source:** Kaggle
- **Creator:** Gerald Piosenka
- **Classes:** 100 Sports Categories
- **Training Images:** 13,492
- **Validation Images:** 500
- **Testing Images:** 500
- **Image Size:** 224 × 224 RGB

---

# 🎯 Objectives

- Develop a Custom CNN for sports image classification.
- Compare Custom CNN with MobileNetV2.
- Evaluate model performance using multiple metrics.
- Visualize model predictions using Explainable AI (Grad-CAM).
- Analyze model errors through misclassified images.

---

# 🧠 Models Implemented

## 1. Custom CNN

- 4 Convolutional Blocks
- Batch Normalization
- Max Pooling
- Global Average Pooling
- Dropout (0.5)
- Softmax Output Layer

## 2. MobileNetV2

Transfer Learning model using MobileNetV2 architecture.

---

# 🔧 Data Preprocessing

- Image Resizing (224×224)
- RGB Images
- Pixel Normalization (0–1)
- Data Augmentation
  - Rotation (20°)
  - Width Shift (20%)
  - Height Shift (20%)
  - Zoom (20%)
  - Horizontal Flip

---

# ⚙️ Training Configuration

| Parameter | Value |
|-----------|-------|
| Optimizer | Adam |
| Learning Rate | 0.001 |
| Loss Function | Categorical Crossentropy |
| Batch Size | 32 |
| Epochs | 15 |
| Early Stopping | Yes |
| Model Checkpoint | Yes |

---

# 📊 Results

## Custom CNN

| Metric | Result |
|---------|--------|
| Test Accuracy | **57.20%** |
| Precision | **61.12%** |
| Recall | **57.20%** |
| F1-score | **53.99%** |

---

## MobileNetV2

| Metric | Result |
|---------|--------|
| Test Accuracy | **1.00%** |

**Note:** MobileNetV2 could not fully utilize pretrained ImageNet weights due to Kaggle network restrictions during execution.

---

# 📈 Generated Outputs

The notebook generates:

- Training Accuracy Curve
- Training Loss Curve
- Confusion Matrix
- Classification Report
- Model Comparison Chart
- Misclassified Images
- Grad-CAM Heatmaps
- Multiple Grad-CAM Examples

---

# 🧠 Explainable AI

Explainability techniques included:

- ✅ Grad-CAM
- ✅ SHAP (attempted)

Grad-CAM successfully highlights the image regions influencing the model's predictions.

---

# 📂 Repository Structure

```
Sports-Image-Classification
│
├── notebooks
│     └── Sports_Image_Classification.ipynb
│
├── models
│     └── custom_cnn_model.keras
│
├── outputs
│     ├── cnn_accuracy.png
│     ├── cnn_loss.png
│     ├── custom_cnn_confusion_matrix.png
│     ├── classification_report.csv
│     ├── model_comparison_chart.png
│     ├── model_comparison.csv
│     ├── misclassified_images.png
│     ├── gradcam_heatmap.png
│     └── multiple_gradcam_examples.png
│
├── README.md
├── requirements.txt
```

---

## Kaggle Notebook

https://www.kaggle.com/code/navaneethnarayan/notebookdb79d8e993

# 🚀 How to Run

1. Clone the repository

```bash
git clone https://github.com/yourusername/Sports-Image-Classification.git
```

2. Install dependencies

```bash
pip install -r requirements.txt
```

3. Open the notebook

```bash
jupyter notebook Sports_Image_Classification.ipynb
```

or upload the notebook to **Kaggle**.

---

# 🛠 Technologies Used

- Python
- TensorFlow / Keras
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- OpenCV
- SHAP

---

# 📌 Future Work

- Fine-tune MobileNetV2 using pretrained ImageNet weights.
- Evaluate EfficientNetB0 and ResNet50.
- Hyperparameter optimization.
- Ensemble learning.
- Vision Transformers (ViT).
- Real-time sports recognition application.

---

# 👨‍🎓 Author

**Navaneeth Narayanan Potty**

University of Europe for Applied Sciences

Machine Learning Project

2026

---

# 📄 License

This project is developed for educational and academic purposes.
