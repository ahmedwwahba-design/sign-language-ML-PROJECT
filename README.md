# 🤟 Sign Language Recognition System (Multi-Model Deep Learning Project)

## 📌 Overview
This project is an advanced Sign Language Recognition system built using both **TensorFlow/Keras** and **PyTorch**.

It classifies hand gesture images into corresponding letters and can also predict full words from sequences of images, with optional **text-to-speech output** using Google Text-to-Speech (gTTS).

The system compares multiple deep learning architectures to achieve the best performance.

---

## 🚀 Key Features
- 🧠 Multi-model training (CNN + Transfer Learning + PyTorch models)
- 📷 Image preprocessing & enhancement pipeline (OpenCV-based)
- ⚡ Fast data generators for efficient training
- 📊 Model comparison and benchmarking
- 🏆 Best model selection automatically
- 📉 Confusion matrix + classification report
- 🔤 Letter-by-letter prediction
- 📝 Word prediction from image sequences
- 🔊 Text-to-speech output (gTTS integration)
- ⚡ GPU support (CUDA enabled training)

---

## 🧠 Models Used

### 🔹 TensorFlow / Keras Models
- Custom CNN (baseline model)
- MobileNetV2 (Transfer Learning)
- EfficientNetB0 (Advanced feature extractor)

### 🔹 PyTorch Models
- ResNet18 (Pretrained)
- ConvNeXt Tiny (State-of-the-art architecture)

---

## 🛠️ Tech Stack
- Python 🐍
- TensorFlow / Keras
- PyTorch
- OpenCV
- NumPy / Pandas
- Scikit-learn
- Matplotlib / Seaborn
- PIL (Pillow)
- gTTS (Google Text-to-Speech)

---

## 📊 Dataset Pipeline
- Dataset loaded from ZIP file
- Automatic extraction and cleaning
- Image filtering (valid formats only)
- Pre-enhancement using OpenCV:
  - Denoising
  - CLAHE contrast enhancement
  - Soft sharpening
  - Gamma correction
- Offline preprocessing for faster training

---

## ⚙️ Training Pipeline
- Train/Validation split (80/20)
- Data augmentation (PyTorch transforms)
- Batch training with generators
- Optimizers:
  - Adam / AdamW
- Learning rate scheduling (OneCycleLR for PyTorch)
- Label smoothing for better generalization

---

## 📈 Evaluation Metrics
- Accuracy (Train & Validation)
- Confusion Matrix
- Classification Report (Precision / Recall / F1-score)
- Model comparison table

---

## 🏆 Best Model Selection
The system automatically selects the best performing model based on validation accuracy.

---

## 🔤 Prediction System

### 📷 Letter Prediction
Each image is classified into a corresponding sign language letter.

### 📝 Word Prediction
Multiple images → sequence → full predicted word.

### 🔊 Speech Output
Predicted word is converted into audio using **gTTS**.

---

## ▶️ How to Run

### 1. Install dependencies
```bash
pip install tensorflow torch torchvision opencv-python-headless matplotlib seaborn scikit-learn gtts pillow
