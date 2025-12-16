# Breast Cancer Classification & Clustering Project

## 📋 Project Overview

This project implements both **supervised** and **unsupervised** machine learning models to analyze the Wisconsin Breast Cancer (Diagnostic) dataset. The goal is to classify tumors as malignant or benign and discover natural patterns in the data through clustering analysis.

## 🎯 Objectives

- Train and evaluate **supervised models** (SVM) for binary classification
- Apply **unsupervised models** (K-Means, Hierarchical, DBSCAN) for pattern discovery
- Compare model performance using various metrics
- Visualize data patterns and model results

## 📊 Dataset

**Source:** Wisconsin Breast Cancer (Diagnostic) Dataset  
**Link:** [Kaggle - Breast Cancer Wisconsin (Diagnostic) Data Set](https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data)  
**Samples:** 569 patients  
**Features:** 30 numerical features computed from cell nuclei characteristics  
**Target:** Diagnosis (M = Malignant, B = Benign)  

### Features Include:
- Radius, texture, perimeter, area, smoothness
- Compactness, concavity, concave points, symmetry, fractal dimension
- Each feature has: mean, standard error, and "worst" (mean of three largest values)

## 🛠️ Technologies Used

- **Python 3.8+**
- **Libraries:**
  - pandas - Data manipulation
  - numpy - Numerical computing
  - scikit-learn - Machine learning models
  - matplotlib - Visualization
  - seaborn - Statistical visualization

## 📁 Project Structure

```
breast-cancer-ml-project/
│
├── data.csv                    # Dataset file
├── visualization.ipynb         # Data exploration & visualization
├── model_training.ipynb        # SVM & clustering implementation
├── README.md                   # This file
└── requirements.txt            # Python dependencies
```

## 🚀 Getting Started

### Prerequisites

```bash
pip install pandas numpy scikit-learn matplotlib seaborn
```

Or install from requirements file:
```bash
pip install -r requirements.txt
```

### Installation

1. Clone or download this repository
2. Place `data.csv` in the project directory
3. Open Jupyter Notebook:
```bash
jupyter notebook
```

### Running the Project

**Step 1: Data Visualization**
- Open `visualization.ipynb`
- Run all cells to explore the dataset
- Review 7 types of visualizations including distributions, correlations, and PCA

**Step 2: Model Training**
- Open `model_training.ipynb`
- Run all cells to train and evaluate models
- Review performance metrics and comparison plots

## 🔬 Models Implemented

### Supervised Learning
- **Support Vector Machine (SVM)**
  - Baseline model with RBF kernel
  - Hyperparameter tuning using GridSearchCV
  - 5-fold cross-validation
  - Performance: ~96-98% accuracy

### Unsupervised Learning
1. **K-Means Clustering**
   - Elbow method for optimal k
   - Silhouette analysis
   
2. **Hierarchical Clustering**
   - Ward linkage method
   - Dendrogram visualization

## 📈 Results Summary

### SVM Classification (Supervised)
- **Accuracy:** ~97%
- **Precision:** ~97%
- **Recall:** ~96%
- **F1-Score:** ~97%
- **ROC-AUC:** ~0.98

### Clustering Performance (Unsupervised)
- **K-Means:** Best overall performance
- **Hierarchical:** Good separation, interpretable dendrogram

## 📊 Visualizations

The project generates:
- Diagnosis distribution plots
- Feature distribution boxplots and violin plots
- Correlation heatmap
- PCA 2D projections
- Confusion matrices
- ROC curves
- Clustering comparison plots
- Dendrogram for hierarchical clustering
- Performance comparison charts

## 🔑 Key Findings

1. **Clear Class Separation:** PCA shows distinct separation between benign and malignant tumors
2. **Feature Importance:** Certain features (radius, perimeter, concave points) are highly discriminative
3. **Model Performance:** SVM achieves excellent classification with proper hyperparameter tuning
4. **Natural Groupings:** Clustering algorithms successfully identify the two main tumor types without labels
5. **Feature Correlation:** Strong correlations exist between related measurements (e.g., radius and perimeter)

## 📝 Evaluation Metrics

### Supervised (Classification)
- Accuracy, Precision, Recall, F1-Score
- ROC-AUC Score
- Confusion Matrix
- Cross-validation scores

### Unsupervised (Clustering)
- Silhouette Score (higher is better)
- Davies-Bouldin Index (lower is better)
- Calinski-Harabasz Score (higher is better)

## 🎓 Educational Value

This project demonstrates:
- Complete machine learning pipeline (data → preprocessing → modeling → evaluation)
- Both supervised and unsupervised learning techniques
- Hyperparameter tuning and model optimization
- Proper train-test splitting and cross-validation
- Multiple evaluation metrics and visualization techniques
- Real-world medical diagnosis application

## 🤝 Team Members

- Francesco Saponara (886465)
- Mattia Chittoni (886462)

## 📧 Contact

For questions or feedback about this project, please contact: f.saponara@campus.unimib.it

---

**Course:** Machine Learning  
**Academic Year:** 2025/2026  
**Due Date:** January 2026  
**Project Type:** Supervised & Unsupervised Learning Analysis