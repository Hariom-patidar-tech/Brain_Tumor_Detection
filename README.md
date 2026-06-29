# 🧠 Brain Tumor Detection and Segmentation using Deep Learning

## 📌 Project Overview

Brain Tumor Detection and Segmentation is a Deep Learning project developed to automatically identify tumor regions from Brain MRI images. The model is based on the **U-Net Architecture**, which is widely used for medical image segmentation.

The application processes MRI slices, predicts tumor regions, and generates a segmentation mask highlighting the detected tumor. A Streamlit web application has also been developed to provide an easy-to-use interface where users can upload MRI scans and visualize the prediction results.

---

# 🎯 Objectives

* Detect brain tumors from MRI images.
* Segment tumor regions accurately.
* Build an end-to-end deep learning pipeline.


---

# 📂 Dataset

Dataset Used:

* BraTS 2020 (Brain Tumor Segmentation Dataset)

Dataset contains:

* MRI Images
* Tumor Masks
* H5 formatted image slices

---

# 🛠 Technologies Used

* Python
* TensorFlow
* Keras
* U-Net
* NumPy
* OpenCV
* Matplotlib
* H5Py


---

# 📊 Project Workflow

```
Brain MRI Dataset
        │
        ▼
Data Loading
        │
        ▼
Image Preprocessing
        │
        ▼
Data Generator
        │
        ▼
Train-Test Split
        │
        ▼
U-Net Model
        │
        ▼
Model Training
        │
        ▼
Model Evaluation
        │
        ▼
Save Trained Model
        │
        ▼
Tumor Prediction
```

---

# 📖 Steps Performed

## 1. Data Loading

* Loaded Brain MRI H5 dataset.
* Read MRI images and segmentation masks.

---

## 2. Data Preprocessing

* Image normalization.
* Binary mask preparation.
* Image resizing.
* Batch generation using custom data generator.

---

## 3. Train-Test Split

Dataset was divided into:

* Training Set
* Validation Set
* Testing Set

---

## 4. Model Architecture

Implemented a U-Net model consisting of:

* Encoder
* Bottleneck
* Decoder
* Skip Connections

The architecture enables precise localization of tumor regions while preserving important spatial information.

---

## 5. Loss Function

Used:

* Binary Cross Entropy
* Dice Loss

Combined as:

```
BCE + Dice Loss
```

---

## 6. Evaluation Metrics

* Dice Coefficient
* IoU Score
* Precision
* Recall
* F1 Score

---

## 7. Model Training

Training includes:

* Early Stopping
* Model Checkpoint
* ReduceLROnPlateau

The model was trained on Brain MRI slices and the best-performing model was saved.

---

## 8. Save Trained Model

Saved Model:

```
brain_tumor_unet.keras
```

Best Model:

```
best_model.keras
```

Kaggle - https://www.kaggle.com/code/hariompatidarr/brain-tumor-detection

---

## 9. Prediction

The trained model performs:

* MRI image loading
* Preprocessing
* Tumor segmentation
* Mask generation
* Overlay visualization

---

image - <img width="521" height="217" alt="image" src="https://github.com/user-attachments/assets/fe1a218f-7b11-4caf-b8e0-90029ebf738c" />
<img width="490" height="363" alt="image" src="https://github.com/user-attachments/assets/1e3e7769-e74a-4d1e-a270-58da54b91cc1" />



---

---

# 🚀 Future Improvements

* Support direct NIfTI (.nii/.nii.gz) MRI uploads.
* 3D Brain MRI segmentation.
* Multi-class tumor segmentation.
* Confidence score visualization.
* Cloud deployment.

---

# 👨‍💻 Author

**Hariom Patidar**

AI & Machine Learning Developer

Specialization:

* Deep Learning
* Computer Vision
* Medical Image Processing
* Image Segmentation


---

# ⭐ If you found this project useful, please consider giving it a Star on GitHub.
