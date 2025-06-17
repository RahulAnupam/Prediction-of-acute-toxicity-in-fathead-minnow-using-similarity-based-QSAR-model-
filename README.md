# Prediction-of-acute-toxicity-in-fathead-minnow-using-similarity-based-QSAR-model
QSAR Oral Toxicity Prediction
This project focuses on predicting the oral toxicity of chemical compounds using machine learning techniques based on molecular descriptors. The dataset is binary classified into toxic and non-toxic compounds.

📁 Dataset
Source: QSAR oral toxicity dataset

Attributes: 1024 binary molecular descriptors and 1 binary target class

Format: CSV with semicolon (;) delimiter, no column headers

📊 Objective
To build a robust classification model that can predict whether a given chemical compound is toxic or non-toxic, using:

Preprocessing and feature scaling

Dataset balancing techniques (SMOTE and random undersampling)

Model training using Random Forest

⚙️ Methodology
1. Data Loading & Preparation
Dataset is loaded using Pandas.

Features (X) and target (y) are separated.

Class distribution is examined before balancing.

2. Handling Imbalanced Data
Applied SMOTE (Synthetic Minority Oversampling Technique) for oversampling.

Used Random UnderSampling to reduce majority class.

Combined them using imblearn.Pipeline.

3. Train-Test Split & Scaling
Stratified train-test split (70-30)

Feature standardization using StandardScaler

4. Modeling
Classifier: Random Forest

Evaluation metrics:

Accuracy

Confusion Matrix

Classification Report

📈 Results
Accuracy and classification metrics are displayed post model evaluation.

Confusion matrix is visualized using Seaborn heatmap.

🛠️ Libraries Used
pandas, numpy

scikit-learn

imbalanced-learn

matplotlib, seaborn

📌 Usage
To run the notebook:

bash
Copy
Edit
pip install pandas scikit-learn imbalanced-learn matplotlib seaborn
Open the notebook in Jupyter:

bash
Copy
Edit
jupyter notebook QSAR_oral_toxicity.ipynb
