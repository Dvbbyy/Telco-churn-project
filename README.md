
Customer Churn Prediction Using Machine Learning
 Project Overview

This project applies machine learning techniques to predict customer churn using real-world telecom data. The goal is to identify customers at risk of leaving and understand key factors influencing churn behavior.

 Objectives
Analyze customer behavior using exploratory data analysis (EDA)
Identify key factors affecting customer churn
Build predictive models to classify churn customers
Compare model performance and interpret results
Provide business insights for customer retention strategies

Dataset

The dataset used in this project is the Telco Customer Churn dataset from:

Kaggle
Dataset includes:

Customer demographics (Age, State, etc.)
Service usage details
Satisfaction Score
Customer Lifetime Value (CLTV)
Churn Label (Target variable)

Tools & Libraries
Python
Pandas
NumPy
Scikit-learn
Matplotlib
Seaborn
Google Colab



# How to Open and Run the Google Colab Notebook

## **1. Open the Notebook**

1. Click the provided Colab link:
    [https://colab.research.google.com/drive/1oQzQdJCyO7KnbKSXxFJ3LX9RWkGE5RWx](https://colab.research.google.com/drive/1oQzQdJCyO7KnbKSXxFJ3LX9RWkGE5RWx)
2. The notebook will open in Google Colab (a cloud-based Python environment).

---

## **2. Make a Copy (Important)**

Before running anything:

1. Click **File → Save a copy in Drive**
2. This ensures you can edit and run your own version without affecting the original.

---

## **3. Install Required Libraries (if needed)**

At the top of the notebook, run any setup cells such as:

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
from sklearn.model_selection import train_test_split
from sklearn.preprocessing import StandardScaler
from sklearn.linear_model import LogisticRegression
from sklearn.ensemble import RandomForestClassifier
from sklearn.metrics import accuracy_score, confusion_matrix, classification_report
```

If any library is missing, install it using:

```python
!pip install package_name
```

---

## **4. Load the Dataset**

Make sure your dataset is uploaded or linked properly:

### Option 1: Upload manually

```python
from google.colab import files
uploaded = files.upload()
```

### Option 2: Load from file path

```python
df = pd.read_csv("your_dataset.csv")
```

---

## **5. Run the Notebook**

1. Run cells one by one using:

   * Play button OR
   * `Shift + Enter`
2. Follow the order from top to bottom:

   * Data loading
   * EDA
   * Preprocessing
   * Model training
   * Evaluation

Do not skip steps, as later cells depend on earlier ones.

---

## **6. View Results**

### EDA Results

You will see:

* Histograms
* Correlation heatmaps
* Bar charts

These help you understand patterns in the dataset.

---

### Model Results

After training models, you will see:

* Accuracy scores
* Confusion matrix
* Precision, recall, and F1-score

Example output:

```python
print(classification_report(y_test, y_pred))
```

---

### Visual Outputs

Graphs such as:

* Feature importance
* Confusion matrix heatmap
* Correlation plots

will display automatically below the code cells.

---

## **7. Save Your Work**

To save results:

* File → Save a copy in Drive
* Or download notebook:

  * File → Download → `.ipynb` or `.pdf`

---

## **8. (Optional) Run All at Once**

You can also run everything using:

```
Runtime → Run all
```

This executes the entire pipeline from start to finish.

---

# Summary

By following these steps, you will:

* Load and explore the dataset
* Run preprocessing steps
* Train ML models
* View performance metrics and graphs

