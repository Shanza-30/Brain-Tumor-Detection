# 🧠 Brain Tumor Detection using Machine Learning

This project demonstrates a **machine learning–based brain tumor detection system** using structured numerical data. The goal is to classify whether a case indicates the presence of a tumor (**1**) or no tumor (**0**) by training and comparing different classification models.


## 📂 Dataset Description

The dataset is synthetically structured and contains the following features:

* **File_Count**: Number of related files or records
* **Description_Length**: Length of the associated textual description
* **Subdirectory (Target Variable)**:

  * `0` → No Tumor
  * `1` → Tumor

The target variable is label-encoded to make it suitable for machine learning classification.



## 🔀 Train–Test Split

* The dataset is split into:

  * **67% Training Data**
  * **33% Testing Data**
* `stratify=y` is used during splitting to ensure **balanced class distribution** across training and testing sets, preventing bias in model evaluation.


## 🧠 Models Used

Two supervised learning models are trained and compared:

### 🌲 Random Forest Classifier

* Ensemble-based model with **100 decision trees**
* Reduces overfitting and improves prediction stability
* Suitable for capturing complex feature interactions

### 🌳 Decision Tree Classifier

* Simple and interpretable model
* Configured with **maximum depth = 3** to avoid overfitting
* Useful for understanding decision rules


## 📊 Prediction & Evaluation

Both models are evaluated on the test dataset using:

* **Accuracy Score**
* **Classification Report**, including:

  * Precision
  * Recall
  * F1-score

This comparison helps identify the model that performs better in terms of overall accuracy and class-wise performance.


## 🛠️ Tools & Technologies

* Python
* Pandas & NumPy
* scikit-learn
* RandomForestClassifier
* DecisionTreeClassifier


## 🔮 Future Improvements

* 🧬 Add medical imaging features (MRI-based pixel data)
* 🤖 Apply deep learning models such as **CNNs** for image-based tumor detection
* 📈 Use cross-validation for more robust evaluation
* ⚖️ Address class imbalance using SMOTE or class weighting
* 🌐 Deploy as a web application using **Flask** or **Streamlit**


## 📌 Conclusion

This project provides a clear comparison between **ensemble** and **tree-based** classifiers for tumor detection. It highlights the importance of model selection, evaluation metrics, and balanced data splitting in healthcare-related machine learning applications.

