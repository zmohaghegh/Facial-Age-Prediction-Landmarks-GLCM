# Facial Age Estimation on FG-NET Dataset

This project implements a robust age estimation pipeline by combining geometric and texture features. It migrates legacy MATLAB methodologies into a modern Python-based workflow.

## 🚀 Key Methodologies
- **Face Detection:** Viola-Jones equivalent using `dlib` frontal face detector.
- **Landmark Detection:** Chehra-style 68-point facial landmark extraction for geometric features.
- **Texture Analysis:** Gray-Level Co-occurrence Matrix (GLCM) to extract skin texture descriptors (Contrast, Homogeneity, Energy, Correlation).
- **Regression Model:** Support Vector Regression (SVR) with an RBF kernel for final age prediction.

## 📊 Performance
- **Dataset:** FG-NET Aging Database
- **Successfully Processed:** 979 images
- **Mean Absolute Error (MAE):** 5.99 years
- **R2 Score:** 0.54

## 🛠️ How to Run
1. Open the `.ipynb` file in Google Colab.
2. The code automatically downloads the FG-NET dataset using `kagglehub`.
3. Ensure the `shape_predictor_68_face_landmarks.dat` is downloaded (automated in script).
4. Run all cells to see the results and performance plots.
