# ML-Driven Fault Diagnosis for Air Compressors

A machine learning framework to diagnose faults in **reciprocating air compressors** using **acoustic-sensor data**. This project classifies compressor states across **7 operating conditions** using extracted time, frequency, and hybrid-domain features.

> Developed as part of the "Artificial Intelligence and Machine Learning" course at IIT Kanpur under the guidance of **Prof. Nishchal K. Verma**.

---

## 🔍 Problem Statement

Reciprocating air compressors often exhibit distinct acoustic signatures under different fault conditions. This project aims to:
- Build a robust classification model using short-duration acoustic recordings (5 seconds).
- Accurately identify the operational state (normal/faulty) of a compressor based on the captured sound.

---

## 📦 Dataset

- **Total Samples**: 1800+ audio recordings  
- **Duration**: 5 seconds per recording  
- **Classes**: 7 fault conditions (including healthy state)  
- **Sensor**: Uniaxial microphone for sound capture  
- **Sampling Rate**: 44.1 kHz (standard)

---

## 🔧 Preprocessing Pipeline

A streamlined pipeline was developed to ensure data quality and consistency:

1. **Clipping** – Remove low-intensity noise at the start/end of recordings  
2. **Smoothing** – Apply filters to reduce short-term fluctuations  
3. **Normalization** – Standardize amplitude across recordings

---

## 📊 Feature Engineering

Extracted **629 acoustic features** from each recording, covering:
- **Time-Domain**: RMS, ZCR, Kurtosis, Crest Factor, etc.
- **Frequency-Domain**: Spectral Centroid, Bandwidth, Entropy
- **Hybrid-Domain**: MFCCs, Energy Entropy, etc.

### Feature Selection
- Applied **mRMR** and **NMIFS** algorithms  
- Reduced to **top 25 discriminative features** for model training

---

## 🤖 Modeling Approach

Trained robust multiclass SVM classifiers using:
- **One-vs-All (OAA)**
- **One-vs-One (OAO)**
- **Directed Acyclic Graph SVM (DAG-SVM)**

### 🏆 Results
- **Accuracy**: 99.5%
- **Inference Time**: <10 seconds

---



