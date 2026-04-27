# DrumRecognizer

# Percussion Audio Classifier using Support Vector Machine

This project implements a supervised learning model based on the Support Vector Machine (SVM) architecture for the automatic classification of percussive audio samples. The system is designed to distinguish between four distinct categories: **Overheads**, **Toms**, **Kicks**, and **Snares**.

## Project Overview

The objective of this application is to transform raw audio signals into numerical feature vectors to enable statistical analysis and classification. By analyzing the timbre and frequency content of each sample, the model achieves high precision in identifying the instrument type.

### Performance
The model currently achieves an accuracy of **93.75%** on the test dataset.

### Technical Features (Feature Extraction)

The following acoustic characteristics are extracted using the `librosa` library to represent each audio sample:

* **Mel-Frequency Cepstral Coefficients (MFCC):** Used to represent the timbre and spectral envelope of the sound.
* **Zero-Crossing Rate (ZCR):** Measures the rate of sign-changes in the signal, which is critical for identifying high-frequency content and noise (common in overheads and snares).
* **Spectral Centroid:** Indicates where the "center of mass" of the spectrum is located, helping the model differentiate between low-frequency sounds (Kicks/Toms) and high-frequency sounds (Overheads).
