🧬 Breast Cancer Diagnosis with K‑Nearest Neighbors

https://img.shields.io/badge/python-3.10-blue.svg
https://img.shields.io/badge/scikit--learn-1.2.2-orange
https://img.shields.io/badge/Jupyter-Notebook-green
https://img.shields.io/badge/License-MIT-yellow.svg

An end‑to‑end machine learning project that predicts whether a breast tumour is benign or malignant using the K‑Nearest Neighbors (KNN) algorithm.
The model achieves 95.6% accuracy and 94.4% F1‑score on the well‑known Wisconsin Diagnostic Breast Cancer (WDBC) dataset.

📖 Overview
Breast cancer is one of the most common cancers among women worldwide. Early and accurate diagnosis is crucial for successful treatment. This project applies a simple yet powerful KNN classifier to distinguish between benign and malignant tumours based on morphological features extracted from fine‑needle aspirate (FNA) images.

The notebook bm.ipynb walks through the complete machine learning pipeline:

Data loading & cleaning

Exploratory data analysis (EDA)

Preprocessing (imputation, scaling)

Model training & hyperparameter selection

Performance evaluation & visualisation

📊 Dataset
Source: UCI Machine Learning Repository – Breast Cancer Wisconsin (Diagnostic)
Instances: 569
Features: 30 numeric features (mean, standard error, and worst values of 10 cell‑nucleus characteristics)
Target:

B (Benign) → 0

M (Malignant) → 1

⚠️ The dataset is already clean – no missing values – but the notebook includes a KNN imputer as a safeguard.

🧪 Project Workflow
Step	Description
1️⃣ Data Loading	Read data.csv and drop the extraneous Unnamed: 32 column.
2️⃣ Train/Test Split	80% training, 20% testing with a fixed random state for reproducibility.
3️⃣ Missing Value Imputation	KNN imputer (n_neighbors=5) – though the dataset is complete.
4️⃣ Feature Scaling	Standardisation (StandardScaler) ensures all features contribute equally to Euclidean distance.
5️⃣ Model Selection	KNN with k = 21 (square root of training size, forced odd to avoid ties).
6️⃣ Evaluation	Confusion matrix, accuracy, F1‑score, recall, and a clear visualisation.
📈 Results
Metric	Score
Accuracy	95.6%
F1‑Score	94.4%
Recall (Malignant)	89.4%
Correct Predictions	109 / 114
The confusion matrix below shows the model’s excellent performance – only 5 misclassifications out of 114 test samples.

https://assets/confusion_matrix.png
If you run the notebook, the plot will be generated automatically.

🛠 Requirements
Python 3.8+

numpy

pandas

scikit‑learn

matplotlib

Install all dependencies with:

bash
pip install -r requirements.txt
(A requirements.txt file is included in the repository.)

🚀 Getting Started
Clone the repository

bash
git clone https://github.com/AliAlsaeed17/Breast-Cancer-Diagnosis-with-K-Nearest-Neighbors
cd breast-cancer-knn
Install dependencies

bash
pip install -r requirements.txt
Launch Jupyter Notebook

bash
jupyter notebook bm.ipynb
Run all cells to reproduce the analysis.

📄 License
This project is open source and available under the MIT License.

👤 Author
Ali Alsaeed
https://img.shields.io/badge/GitHub-100000?style=flat&logo=github&logoColor=white
https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white

⭐ If you find this project useful, please consider giving it a star! ⭐
