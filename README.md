# Music Genre Classification using CNN Feature Extraction and Classical ML

This project is a faithful implementation of the paper:

> *Combining Convolutional Neural Networks and Classical Machine Learning Algorithms for Music Genre Classification*

The work demonstrates how a compact CNN can learn meaningful audio representations that outperform raw MFCC and PCA-based features when combined with classical classifiers.

---

## 📊 Dataset
- **GTZAN Dataset**
- 5 genres: Classical, Blues, Pop, Hip-Hop, Metal
- 500 audio samples (400 train / 100 test)
- Accessed using `kagglehub`

---

## 🔍 Feature Representation
- MFCC (20 coefficients, 1290 time frames)
- MFCC heatmap visualization
- CNN activation heatmaps

---

## 🧠 Model Architecture
- 2-layer Dilated 1D CNN
- Average pooling + Dropout + Batch Normalization
- Feature extraction after second pooling layer
- Final CNN feature vector size: **48**

---

## 🤖 Models Compared
- Logistic Regression
- Support Vector Machine (RBF)
- Random Forest

Baselines:
- Raw MFCC
- PCA (50 components)

---

## 📈 Key Results
| Model | Accuracy |
|------|----------|
| Raw MFCC + RF | ~0.78 |
| PCA MFCC + RF | ~0.79 |
| CNN Only | ~0.88 |
| **CNN Features + RF** | **~0.88** |


## 📌 Key Insight
CNN-learned features generalize better than both raw MFCC and PCA features when used with classical machine learning models.



