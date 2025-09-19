# 🎓 Student Success Prediction using Machine Learning

## 📌 Overview
This project predicts whether a student will **pass or fail** using different machine learning models.  
We trained and tested models on a real dataset to evaluate their performance.

## 🗂 Dataset
- **Source**: [UCI Student Performance Dataset](https://archive.ics.uci.edu/ml/datasets/student+performance)  
- **Features**: demographic, social, and academic attributes  
- **Target**: Pass (1) / Fail (0)

## 🤖 Models Used
- Decision Tree Classifier 🌳  
- K-Nearest Neighbors (KNN) 👥  
- Support Vector Machine (SVM) ⚡  

## 📊 Results

| Metric                | Decision Tree (Before Pruning) | Decision Tree (After Pruning) | KNN   | SVM   |
|------------------------|--------------------------------|--------------------------------|-------|-------|
| Confusion Matrix       | [42  4]<br>[ 9 64]            | [45  1]<br>[10 63]            | [17 29]<br>[ 4 69] | [40  6]<br>[ 8 65] |
| Precision (Class 0)    | 0.82                           | 0.82                           | 0.81  | 0.83  |
| Recall (Class 0)       | 0.91                           | 0.98                           | 0.37  | 0.87  |
| F1-Score (Class 0)     | 0.87                           | 0.89                           | 0.51  | 0.85  |
| Precision (Class 1)    | 0.94                           | 0.98                           | 0.70  | 0.92  |
| Recall (Class 1)       | 0.88                           | 0.86                           | 0.95  | 0.89  |
| F1-Score (Class 1)     | 0.91                           | 0.92                           | 0.81  | 0.90  |
| **Accuracy**           | **0.89**                       | **0.91**                       | **0.72** | **0.88** |
✅ The **Decision Tree (After Pruning)** achieved the best performance among all models.
## 🚀 How to Run
```bash
# Clone the repository
git clone https://github.com/username/student-success-ml.git
cd student-success-ml

# Install dependencies
pip install -r requirements.txt

# Run the notebook
jupyter notebook Student_Success_Prediction.ipynb
