# PCOS-Ultrasound-Image-Analysis
Computer vision based analysis of PCOS ultrasound images using cyst detection and texture features


## 📌 Project Overview
This project focuses on analyzing ovarian ultrasound images to identify cyst-like structures associated with Polycystic Ovary Syndrome (PCOS) using computer vision techniques.

Instead of directly classifying images, the project emphasizes **image enhancement, cyst detection, and feature extraction** to support medical image analysis.

---

## 🧠 Methodology

### 1. Image Preprocessing
- Converted ultrasound images to grayscale
- Applied **CLAHE (Contrast Limited Adaptive Histogram Equalization)** to enhance contrast
- Reduced noise using Gaussian blur

### 2. Cyst Candidate Detection
- Applied thresholding to isolate dark cyst regions
- Used morphological operations to remove noise
- Detected contours and filtered them based on area constraints

### 3. Feature Extraction
Extracted meaningful features from each image:
- Number of cyst-like regions
- Mean cyst area
- Area ratio (cyst area / image area)
- Texture features (contrast, homogeneity) using **GLCM**

### 4. Visualization
- Generated overlay images with bounding boxes around detected cysts
- Compared original, enhanced, and detected images visually

---

## 📊 Technologies Used
- Python
- OpenCV
- NumPy, Pandas
- Matplotlib, Seaborn
- scikit-image (GLCM)

---

## ⚠️ Disclaimer
This project is intended for **academic and research purposes only** and is **not a medical diagnostic tool**.

---

## 🚀 Future Improvements
- Deep learning based segmentation (U-Net)
- Expert-validated cyst annotations
- Multi-dataset generalization
