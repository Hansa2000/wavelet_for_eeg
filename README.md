# README: Wavelet Signal Processing Project

## Overview
This project reimplements the paper **"A Comparative Study of Wavelet Families for EEG Signal Classification"** by Gandhi et al. (2011). It focuses on using Discrete Wavelet Transform (DWT) to classify epileptic EEG signals, evaluating wavelet families, and improving classification techniques.

---

## Objectives
1. Reproduce the paper's methodology and results.
2. Extract features from DWT coefficients (e.g., energy, entropy, standard deviation).
3. Compare classifiers like SVM, PNN, Gaussian Naive Bayes, and CNNs.
4. Explore improvements in feature extraction and classifier performance.

---

## Dataset
- **Andrzejak EEG Dataset**
  - Contains five sets (A-E) of EEG signals.
  - **A & B:** Healthy individuals (eyes open/closed).
  - **C, D & E:** Epileptic patients (seizure-free and seizure segments).

---

## Methodology
1. **Wavelet Transform:** Used DWT with different wavelet families (e.g., Coiflets, Daubechies).
2. **Feature Extraction:** Computed features like energy, entropy, and kurtosis.
3. **Classification:** Evaluated classifiers (SVM, PNN, Gaussian Naive Bayes, CNN).

---

## Results
1. **Best Wavelet:** Coiflets (Coif1) performed the best.
2. **Optimal Features:** Energy and kurtosis provided high accuracy.
3. **Classifier Performance:** CNN with attention achieved near-perfect results.
4. **Efficiency:** Improvements in computational time and edge-device suitability.

---

## Challenges
1. Lack of details in the original paper required assumptions.
2. Custom implementation for PNN due to unavailable libraries.

---

## How to Run
1. **Clone Repository:**
   ```bash
   git clone <repository-url>
   cd <project-directory>
   ```
2. **Install Dependencies:**
   ```bash
   pip install -r requirements.txt
   ```
3. **Run Script:**
   ```bash
   python main.py
   ```

---

## References
1. Gandhi, T., et al. (2011). *A comparative study of wavelet families for EEG signal classification*. Neurocomputing.
2. Andrzejak, R. G., et al. (2001). *Indications of nonlinear deterministic structures in EEG time series.*
