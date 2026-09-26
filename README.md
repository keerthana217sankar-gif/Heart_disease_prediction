# Heart Disease Prediction Using Machine Learning

## 📌 Project Overview

This project demonstrates a simple machine learning approach for predicting heart disease using patient-related health features.

The project uses **Logistic Regression** and **K-Nearest Neighbors (KNN)** classification algorithms and evaluates their performance using different classification metrics.

> **Note:** This is an educational machine learning project based on a very small dataset. It is not intended for real-world medical diagnosis or clinical use.

## 📊 Dataset

The dataset is stored in:

```text
heartdisease.csv
```

The dataset contains the following features:

| Feature    | Description                       |
| ---------- | --------------------------------- |
| `age`      | Age of the patient                |
| `sex`      | Sex encoded as a numerical value  |
| `cp`       | Chest pain type                   |
| `trestbps` | Resting blood pressure            |
| `chol`     | Cholesterol level                 |
| `fbs`      | Fasting blood sugar indicator     |
| `thalach`  | Maximum heart rate achieved       |
| `exang`    | Exercise-induced angina indicator |
| `oldpeak`  | ST depression value               |
| `ca`       | Number of major vessels           |
| `target`   | Target class for prediction       |

The `target` column is used as the output variable, while the remaining columns are used as input features.

## 🛠️ Technologies Used

* Python
* Jupyter Notebook
* Pandas
* Scikit-learn
* Matplotlib
* Seaborn

## 🤖 Machine Learning Algorithms

### 1. Logistic Regression

Logistic Regression is used as the first classification model to predict the target class.

The model is evaluated using:

* Accuracy
* Precision
* Recall
* F1-score
* Confusion Matrix

### 2. K-Nearest Neighbors (KNN)

KNN is also used for classification.

Different values of `K` are tested:

```text
K = 1
K = 3
K = 5
K = 7
K = 9
```

The notebook compares the accuracy obtained for each value of K.

## 🔄 Project Workflow

```text
Load Dataset
     ↓
Explore Dataset
     ↓
Separate Features and Target
     ↓
Split Data into Training and Testing Sets
     ↓
Train Logistic Regression Model
     ↓
Make Predictions
     ↓
Evaluate Model
     ↓
Train KNN Model
     ↓
Test Different K Values
     ↓
Compare Results
```

## 📈 Results

### Logistic Regression

The current notebook produced the following results:

| Metric    | Score |
| --------- | ----: |
| Accuracy  |  0.25 |
| Precision |  0.33 |
| Recall    |  0.50 |
| F1-score  |  0.40 |

Confusion Matrix:

```text
[[0 2]
 [1 1]]
```

### KNN

The observed accuracy for different K values was:

|  K | Accuracy |
| -: | -------: |
|  1 |     0.25 |
|  3 |     0.25 |
|  5 |     0.50 |
|  7 |     0.50 |
|  9 |     0.50 |

Based on these results, KNN with `K = 5`, `K = 7`, and `K = 9` achieved the highest accuracy in this experiment.

## 📁 Project Structure

```text
heart-disease-prediction/
│
├── heart_disease_prediction.ipynb
├── heartdisease.csv
└── README.md
```

## 🚀 How to Run the Project

### Step 1: Clone the Repository

```bash
git clone https://github.com/YOUR-USERNAME/heart-disease-prediction.git
```

### Step 2: Open the Project Folder

```bash
cd heart-disease-prediction
```

### Step 3: Install Required Libraries

```bash
pip install pandas scikit-learn matplotlib seaborn jupyter
```

### Step 4: Start Jupyter Notebook

```bash
jupyter notebook
```

### Step 5: Open the Notebook

Open:

```text
heart_disease_prediction.ipynb
```

Make sure `heartdisease.csv` is in the same folder as the notebook.

Run the notebook cells from top to bottom.

## 📌 Future Improvements

This project can be improved by:

* Using a larger heart disease dataset
* Performing data preprocessing and feature scaling
* Handling missing values
* Using cross-validation
* Testing additional machine learning algorithms
* Performing hyperparameter tuning
* Comparing models using multiple evaluation metrics
* Improving model visualization

## ⚠️ Disclaimer

This project is created for **educational and learning purposes only**.

The dataset used is very small, and the model performance is not sufficient for medical decision-making. The predictions should not be used as a substitute for professional medical advice.

## 👩‍💻 Author

**Your Name**

GitHub: `https://github.com/YOUR-USERNAME`
