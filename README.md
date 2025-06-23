# -Acoustic-Fault-Diagnosis-for-Air-Compressors
**Overview**-

This project demonstrates a machine learning pipeline for early detection of faults in reciprocating air compressors using acoustic signals. By processing sound recordings from a single optimized sensor location, the system predicts one of eight machine states (healthy + 7 fault modes) to support proactive, data-driven maintenance.

**Key Features**

Sensor Placement: Applied Empirical Mode Decomposition (EMD) and envelope analysis to identify the most informative microphone location.

Data Pipeline: Preprocessed 1,800+ recordings through filtering, clipping, smoothing, and normalization for consistent, high-quality input.

Feature Engineering: Extracted 629 metrics across time, frequency, and time–frequency domains (FFT, DWT, WPT, STFT, DCT, etc.).

Dimensionality Reduction: Used mRMR/NMIFS to select a 25-variable subset, reducing compute time by 95% while retaining ~98% classification accuracy.

Modeling: Evaluated SVM classifiers over held-out data, achieving sub-10s prototype inference and validating feasibility for proactive maintenance planning.
