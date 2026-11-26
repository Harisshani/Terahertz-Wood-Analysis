


Terahertz and X-Ray Wood Analysis

This repository contains my internship project at **CSIR-CEERI**, focused on non-destructive wood analysis using Terahertz (THz) and X-ray imaging techniques.  
The project explores defect detection, eature extraction, and machine learning models for predicting wood density in tropical and diverse wood species.

---

Project Overview
The project is divided into three phases:

Phase 1 – Defect Detection
- Pixel-level temporal analysis of THz signals.
- Identification of defects (holes) using **standard deviation (STD)** and variation patterns.
- Visualization of anomaly regions across wood samples.

Phase 2 – Density Prediction Using THz Data
- Feature extraction:
  - Temporal statistics
  - FFT-based spectral features
  - Hybrid statistical–spectral features
- Machine learning models:
  - Random Forest
  - XGBoost
  - Stacked Ensemble Regressor (RF + XGBoost + Ridge)
- Performance:
  - Tropical dataset: R² = 0.9985, MAE ≈ 4.7 kg/m³
  - Diverse dataset: R² = 0.9992, MAE ≈ 4.6 kg/m³

Phase 3 – Density Prediction Using X-Ray & Physical Properties
- Utilized X-ray image features along with physical data:
  - Mass
  - Volume
  - Moisture content
- Models:
  - Random Forest
  - Stacked Ensemble (CatBoost + XGBoost + RF with Ridge)
- Performance:
  - Diverse dataset: R² = 0.9997, MAE ≈ 2.7 kg/m³
  - Tropical dataset: R² = 0.9985, MAE ≈ 4.7 kg/m³

---

Dataset
- Total of 110 wood samples:
  - 78 diverse species
  - 32 tropical species
- From the publication:  
  Non-Destructive Wood Analysis Dataset: Comparing X-Ray and Terahertz Imaging Techniques.

---

Technologies & Tools
- Python (NumPy, Pandas, Scikit-learn, Matplotlib, SciPy)
- Machine Learning: Random Forest, XGBoost, CatBoost, Stacking Regressors
- Signal Processing: FFT, temporal statistics, pixel-level sampling
- Cross-validation: Leave-One-Species-Out (LOSO-CV)

---

Results
- Near-perfect density prediction accuracy.
- Robust defect detection using temporal STD-based pixel analysis.
- Demonstrated complementary strengths of THz and X-ray imaging techniques.


