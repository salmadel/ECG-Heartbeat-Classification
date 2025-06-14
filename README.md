# 🫀 ECG Heartbeat Classification using 1D CNN

## Project Overview

This project leverages a 1D Convolutional Neural Network (1D-CNN) to classify ECG (electrocardiogram) heartbeat signals into five categories. The model identifies temporal patterns within the ECG waveform, aiding in the detection and diagnosis of various heart arrhythmias.

![ECG](https://github.com/user-attachments/assets/77900d89-bbff-43d5-b588-0e5572a30e10)


## Dataset Overview

The dataset contains pre-segmented ECG heartbeat signals, each with 187 time steps. These are derived from well-known sources like the MIT-BIH Arrhythmia dataset.
- [Dataset Link](https://www.kaggle.com/datasets/shayanfazeli/heartbeat)

- Classification Categories:

| Label | Class | Description                                      | Percentage  |
|:-----:|:----: |:------------------------------------------------:| :---------- |
|  0    |  N    | Normal beat                                      | 82.8%       |
|  1    |  S    | Supraventricular ectopic beat                    | 2.5%        |
|  2    |  V    | Ventricular ectopic beat                         | 6.6%        |
|  3    |  F    | Fusion beat (blend of normal and abnormal)       | 0.7%        |
|  4    |  Q    | Unknown or unclassifiable beat                   | 7.3%        |




## Technologies & Libraries

- **Python**
- **TensorFlow / Keras** – Deep learning framework
- **NumPy, Pandas** – Data manipulation
- **Scikit-learn** – Evaluation metrics, preprocessing
- **Matplotlib, Seaborn** – Visualizations


## Project Workflow

1. **Data Preprocessing**
   
   - Train-test split (stratified)
   - Scaling of ECG signals
   - Class distribution analysis and weighting for imbalance

2. **Model Architecture**
   - Stacked 1D Convolutional layers with ReLU activation
   - MaxPooling & Dropout for regularization
   - Dense layers with Softmax output for multiclass classification

3. **Training**
   - Optimizer: Adam
   - Loss: Sparse Categorical Crossentropy
   - Evaluation using validation split and model checkpoints

4. **Evaluation**
   - Metrics: Accuracy, Precision, Recall, F1-score
   - Confusion matrix visualization
   - Training curves for loss and accuracy


## Results
- Accuracy : 93.09%
- Precision : 96.44%
- Recall   : 93.09%
- F1 Score : 94.25%
- Training Accuracy & Loss Curves : 
![Loss Accuracy](https://github.com/user-attachments/assets/8e7f176c-96f8-4fd3-82d8-1106d9f01c6d)

- Confusion Matrix :
  ![CM](https://github.com/user-attachments/assets/d9dfa732-7107-4a93-a0bb-e872baf5debb)


  
