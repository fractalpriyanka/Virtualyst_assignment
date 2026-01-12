# Handwritten Digit Classification using Classical Machine Learning

## 📌 Project Overview
This project implements an **end-to-end machine learning pipeline** to classify grayscale images of handwritten digits (0–9) using **classical machine learning algorithms**. The dataset used is the MNIST handwritten digits dataset in CSV format, where each image is represented as a flattened 28×28 pixel vector.

The project focuses on **data preprocessing, dimensionality reduction, model training, evaluation, and error analysis**, without using any pre-trained models or neural networks.

---

## 🎯 Objective
- Classify handwritten digits (0–9) from grayscale images.
- Implement and compare classical ML models:
  - K-Nearest Neighbors (KNN)
  - Support Vector Machine (SVM)
  - Decision Tree
- Evaluate performance using accuracy and confusion matrices.
- Analyze misclassifications and improve performance using PCA.

---

## 📂 Dataset Description
- **Dataset:** MNIST (CSV format)
- **Samples:** 10,000
- **Features:** 784 pixel values (28×28 flattened)
- **Labels:** Digits from 0 to 9
- **Pixel Range:** 0–255

Each row in the dataset represents a single image along with its corresponding digit label.

---

## 🛠️ Tools & Libraries Used
- Python
- NumPy
- Pandas
- scikit-learn
- Matplotlib
- Seaborn

> ⚠️ No pre-trained models, deep learning frameworks, or managed cloud platforms were used.

---

## 🔄 Project Workflow
1. Data Loading & Exploration  
2. Data Preprocessing & Normalization  
3. Dimensionality Reduction using PCA (Optional)  
4. Model Training (Baseline & PCA-based)  
5. Model Evaluation  
6. Error Analysis  
7. Final Reporting  

---

## 📊 Models Implemented

### Baseline Models (Without PCA)
| Model | Accuracy |
|------|----------|
| KNN (k = 3) | 0.955 |
| SVM (Linear) | 0.927 |
| SVM (RBF) | 0.968 |
| Decision Tree | 0.8125 |

### PCA-Based Models
| Model | PCA Components | Accuracy |
|------|---------------|----------|
| KNN | 50 | 0.959 |
| KNN | 100 | 0.9545 |
| SVM (RBF) | 50 | **0.975** |
| SVM (RBF) | 100 | 0.9745 |

---

## 📈 Evaluation Metrics
- Accuracy Score
- Confusion Matrix (Heatmap Visualization)
- Misclassified Image Analysis

---

## 🔍 Error Analysis
- Most misclassifications occur between visually similar digits such as:
  - 3 ↔ 5
  - 4 ↔ 9
  - 1 ↔ 7
- Decision Tree struggled the most due to overfitting on raw pixel features.
- SVM (RBF) with PCA produced the cleanest confusion matrix and best generalization.

---

## 🧠 Key Insights
- **SVM (RBF) + PCA** achieved the best performance.
- PCA reduced noise and redundant pixel correlations.
- Distance-based models like KNN are sensitive to dimensionality.
- Classical ML models lack spatial awareness, causing confusion between similar digit shapes.

---


---

## ▶️ How to Run the Project

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/handwritten-digit-classification.git
cd handwritten-digit-classification

python -m venv venv
venv\Scripts\activate

pip install -r requirements.txt
```

📄 Assignment Compliance

✔ Classical ML models only
✔ No neural networks or pre-trained models
✔ Full evaluation and analysis
✔ PCA experiments included
✔ Submission-ready report



