# 😷 Face Mask Detection using Deep Learning

A deep learning-based computer vision project that detects whether a person is wearing a face mask or not in real-time using OpenCV, TensorFlow, and Keras. This project aims to contribute to public safety by enabling mask compliance monitoring, especially during situations like the COVID-19 pandemic.

---

## 📌 Features

- ✅ Real-time face mask detection using webcam  
- ✅ Detects multiple faces in a single frame  
- ✅ Trained on a dataset with and without masks  
- ✅ Built using MobileNetV2 for efficient performance  
- ✅ Easy-to-use and modify for real-world deployment  

---

## 🧠 Model Architecture

- **Base Model:** MobileNetV2 (Pre-trained on ImageNet)  
- **Custom Layers:** Fully connected dense layers for binary classification (with_mask / without_mask)  
- **Loss Function:** Binary Crossentropy  
- **Optimizer:** Adam  
- **Evaluation Metric:** Accuracy  

---

## 🗃️ Dataset

Dataset used: [Face Mask Dataset by Prajna Bhandary](https://github.com/prajnasb/observations/tree/master/experiements/data)

- Two classes: `with_mask` and `without_mask`  
- Preprocessing includes:
  - Image resizing (224x224)
  - Normalization
  - Data augmentation for robustness  

---

## 🛠️ Technologies Used

- **Language:** Python 🐍  
- **Libraries/Frameworks:**  
  - TensorFlow / Keras  
  - OpenCV  
  - NumPy  
  - Scikit-learn  
  - Matplotlib  

---

## 🚀 Installation

### 1. Clone the repository

```bash
git clone https://github.com/Raj140503/Face-Mask-Detection.git
cd Face-Mask-Detection
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Run real-time mask detection
```bash
python detect_mask_video.py
```
---

## 📁 Project Structure
```bash
Face-Mask-Detection/
│
├── dataset/                  # Input images (with_mask / without_mask)
├── face_detector/            # Caffe-based face detection model
├── examples/                 # Example outputs and visuals
├── detect_mask_image.py      # Detect masks on static images
├── detect_mask_video.py      # Detect masks in real-time via webcam
├── train_mask_detector.py    # Model training script
├── mask_detector.model       # Trained face mask detection model
├── requirements.txt          # Python dependencies
└── README.md                 # Project documentation
```
---

## ✅ Results
- Achieved ~95% accuracy on validation data
- Stable performance in real-time with multiple faces
- Accurate even under different lighting conditions
---

## 💡 Future Improvements
- Integrate alert system for no-mask detection
- Deploy the model on edge devices (Raspberry Pi, Jetson Nano)
- Improve mask dataset for more variety (different angles, mask types)
- Web or mobile app deployment for public use
---

**Developed by [Raj140503](https://github.com/Raj140503)**
