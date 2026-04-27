# Diabetic Retinopathy Classification using Machine Learning

## 📌 Overview
This project presents a machine learning-based system for the automated classification of diabetic retinopathy (DR) using retinal fundus images. The goal is to assist early diagnosis by reducing reliance on manual and subjective clinical assessment.

The system focuses on feature engineering and classical machine learning techniques instead of deep learning, ensuring interpretability and lower computational cost.

---

## ⚙️ Methodology

### 1. Image Preprocessing
- Conversion to grayscale
- Image resizing (128×128)
- Contrast enhancement
- Noise reduction

### 2. Feature Engineering
A comprehensive set of features is extracted:

- **Statistical Features**: Mean, standard deviation, skewness, kurtosis  
- **Texture Features**: GLCM, Local Binary Patterns (LBP)  
- **Edge Features**: Edge density using Sobel/Canny  
- **Frequency Features**: Fourier Transform energy  
- **Entropy & Gradient Features**

### 3. Dimensionality Reduction
- Principal Component Analysis (PCA)
- Retains **99% variance**

### 4. Machine Learning Models
The following models are implemented and compared:
- K-Nearest Neighbours (KNN)
- Naive Bayes
- Minimum Distance Classifier
- Support Vector Machine (SVM)
- Random Forest

---

## 📊 Results

| Model              | Accuracy |
|------------------|---------|
| KNN              | 83.33%  |
| Naive Bayes      | 75.24%  |
| Minimum Distance | 90.00%  |
| SVM              | 92.38%  |
| Random Forest    | 94.76%  |

- Random Forest achieved the best performance  
- Feature engineering significantly improved classification accuracy  
- PCA helped reduce complexity while maintaining performance  

---

## 📈 Key Features
- Multi-class classification (7 DR stages)
- Data augmentation to handle class imbalance
- Statistical and inferential analysis of features
- Advanced visualisations (PCA plots, confusion matrix, heatmaps)

---

## 💻 Implementation
- Developed in **MATLAB**
- No reliance on built-in machine learning shortcuts
- Fully reproducible pipeline from preprocessing to classification

---

## ▶️ How to Run
1. Open MATLAB
2. Ensure dataset path is correctly set
3. Run:
   ```matlab
   main.m
