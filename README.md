# Machine Learning & Computer Vision Repository

Welcome to this comprehensive repository featuring multiple machine learning and computer vision projects. This space serves as a portfolio of data science workflows ranging from tabular data regression to advanced image segmentation.

## 📁 Repository Structure

The repository is organized into two primary modules:

### 1. [Score Prediction](./score%20prediction/)
**Focus**: Student Academic Performance Analysis
- **Goal**: Predicting student final grades (G3) based on demographic, social, and academic factors.
- **Key Files**:
    - [`Student_Performance_Analysis.ipynb`](./score%20prediction/Student_Performance_Analysis.ipynb): A complete pipeline featuring EDA, feature engineering, and a comparison of 10 regression models (Linear, Random Forest, XGBoost, etc.).
    - `student-mat.csv` & `student-por.csv`: Specialized datasets for Math and Portuguese courses.
- **Highlights**: Achieves up to **82.7% R²** accuracy when intermediate grades are included, and identifies "absences" and "previous failures" as critical predictors for student success.

### 2. [Image Classification & Segmentation](./Image%20classification/)
**Focus**: Industrial Defect Detection (MVTec Dataset)
- **Goal**: Identifying and localizing structural and surface defects in manufacturing products (metal nuts).
- **Key Files**:
    - [`CNN_Defect_Segmentation.ipynb`](./Image%20classification/CNN_Defect_Segmentation.ipynb): High-precision **Semantic Segmentation** using the **U-Net architecture** to generate pixel-level defect masks.
    - [`Unsupervised_Learning_Clustering.ipynb`](./Image%20classification/Unsupervised_Learning_Clustering.ipynb): **Anomaly Detection** using unsupervised methods (VGG16 Transfer Learning + PCA + K-means/DBSCAN).
- **Highlights**: Combines deep learning for precise localization with classical unsupervised clustering for generalized anomaly detection.

---

## 🚀 Getting Started

### Prerequisites
To run the notebooks in this repository, you will need:
- Python 3.8+
- Jupyter Notebook / Lab
- Libraries: `tensorflow`, `scikit-learn`, `pandas`, `numpy`, `matplotlib`, `seaborn`

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/NividDesai/Machine-Learning_score_prediction.git
   ```
2. Navigate to the desired project folder:
   ```bash
   cd "score prediction"  # or "Image classification"
   ```

## 📊 Summary of Technical Skills
- **Deep Learning**: CNNs, U-Net Architecture, Transfer Learning (VGG16).
- **Classical ML**: Regression (10+ variants), Clustering (K-means, DBSCAN).
- **Data Engineering**: Feature scaling, Dimensionality Reduction (PCA, t-SNE).
- **Analysis**: Exploratory Data Analysis (EDA), Hyperparameter Tuning, Feature Importance analysis.

