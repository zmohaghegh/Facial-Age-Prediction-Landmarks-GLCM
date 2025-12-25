# Age Prediction based on Facial Landmarks and Texture Features

This project implements a hybrid approach for age estimation by combining **Geometric (Facial Landmarks)** and **Texture (GLCM)** features using Support Vector Regression (SVR).

## 📌 Key Methodology
1. **Facial Landmarks:** Locating 68 specific feature points (eyes, nose, mouth, jawline) to capture morphological changes in the face over time.
2. **Texture Analysis (GLCM):** Using the Gray-Level Co-occurrence Matrix to extract spatial gray-level dependence, capturing skin texture and wrinkle patterns.
3. **Face Detection:** Based on the classic **Viola-Jones** algorithm (Haar features).
4. **Regression:** Implementing **SVM Regression** to map the high-dimensional feature vector to a continuous age value.

## 🚀 Research Findings
- **Landmarks vs. Texture:** Morphology (landmarks) generally reflects age better than simple texture.
- **Hybrid Performance:** Combining both feature sets significantly improves prediction accuracy compared to using either alone.

## 🛠️ Implementation Details
- **GLCM Parameters:** Angles (0°, 45°, 90°, 135°) with reduced gray levels (16 levels) for computational efficiency.
- **Kernel:** RBF (Radial Basis Function) for SVR to handle non-linear age-related facial transformations.

## 💻 Tech Stack
- Python (Scikit-learn, Scikit-image)
- OpenCV (for Viola-Jones implementation)
- Matplotlib (for analytical plots)
