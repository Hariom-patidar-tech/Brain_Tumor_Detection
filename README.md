# 🧠 Brain Tumor Detection and Segmentation using Deep Learning

## 📌 Project Overview

Brain Tumor Detection and Segmentation is a Deep Learning project developed to automatically identify tumor regions from Brain MRI images. The model is based on the **U-Net Architecture**, which is widely used for medical image segmentation.

The application processes MRI slices, predicts tumor regions, and generates a segmentation mask highlighting the detected tumor. A Streamlit web application has also been developed to provide an easy-to-use interface where users can upload MRI scans and visualize the prediction results.

---

# 🎯 Objectives

* Detect brain tumors from MRI images.
* Segment tumor regions accurately.
* Build an end-to-end deep learning pipeline.
* Deploy the trained model using Streamlit.

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
* Streamlit

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
Streamlit Deployment
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

---

## 9. Prediction

The trained model performs:

* MRI image loading
* Preprocessing
* Tumor segmentation
* Mask generation
* Overlay visualization

---

# 💻 Streamlit Application

The project also includes a Streamlit-based web application.

Features:

* Upload MRI Image
* Automatic Preprocessing
* Tumor Prediction
* Segmentation Mask
* Overlay Visualization
* User-friendly Interface

Run locally:

```bash
streamlit run app.py
```

---

# 📁 Project Structure

```
Brain-Tumor-Detection/

│── app.py
│── brain_tumor_unet.keras
│── best_model.keras
│── requirements.txt
│── README.md

├── sample_data/

├── notebooks/
│     Brain_Tumor_Detection.ipynb

├── images/

└── outputs/
```

---

# 📦 Installation

Clone the repository

```bash
git clone YOUR_GITHUB_REPOSITORY
```

Move into the project folder

```bash
cd Brain-Tumor-Detection
```

Create virtual environment

```bash
python -m venv venv
```

Activate environment

Windows

```bash
venv\Scripts\activate
```

Install dependencies

```bash
pip install -r requirements.txt
```

Run the application

```bash
streamlit run app.py
```

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
* Streamlit Deployment

---

# ⭐ If you found this project useful, please consider giving it a Star on GitHub.
