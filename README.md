# 🧠 Dual-Stage Deep Learning System for Brain Tumor Segmentation and Classification

A modular deep learning pipeline combining U-Net-based segmentation and CNN-based classification to detect and classify brain tumors from MRI images.


## 📌 Project Highlights

- 🔍 **Tumor Segmentation** using U-Net on grayscale MRI images  
- 🧠 **Tumor Classification** using CNN (4 classes: No Tumor, Glioma, Meningioma, Pituitary)  
- ⚙️ Dual-stage system mimics clinical workflow  
- 📈 High performance: Dice Score of 0.89, Classification Accuracy of 94.5%  
- 🧪 Built with TensorFlow/Keras, OpenCV, NumPy  

---
## 🔬 System Architecture

### ➤ Stage 1: U-Net Segmentation Model

- **Input:** Grayscale MRI
- **Output:** Binary tumor mask
- **Loss:** Binary Cross-Entropy + Dice Loss  
- **Framework:** TensorFlow/Keras

### ➤ Stage 2: CNN Classification Model

- **Input:** Masked applied tumor image
- **Output:** Tumor Class (4 categories)
- **Loss:** Categorical Cross-Entropy  
- **Architecture:** Convolutional layers + Fully Connected Layers

---

## 🧪 Dataset Overview

### Dataset 1 – Segmentation

- Format: Grayscale `.jpg` / `.png`
- Labels: 0 - No Tumor, 1 - Glioma, 2 - Meningioma, 3 - Pituitary  
- Preprocessing: Resize, Normalization, Augmentation

### Dataset 2 – Classification

- Format: RGB MRI images  
- Classes: Same as above  
- Preprocessing: Resize, Normalize, Label Encoding

---

## 🧰 Tools & Technologies

- `TensorFlow`, `Keras`, `OpenCV`, `Matplotlib`
- `NumPy`, `scikit-learn`, `Pandas`

---

## 📊 Results

| Task             | Metric           | Score     |
|------------------|------------------|-----------|
| Segmentation     | Dice Score       | 0.89      |
| Classification   | Accuracy         | 94.5%     |

![image](https://github.com/user-attachments/assets/dfaab99c-0861-4ef6-8ddb-d26fc52b507b)
![image](https://github.com/user-attachments/assets/947afd76-7fae-41c1-b5ba-d38a6f7332a7)
![image](https://github.com/user-attachments/assets/41511a06-35ec-43a8-82c2-8367ccab9fd4)

---
