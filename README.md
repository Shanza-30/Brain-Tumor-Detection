# Brain-Tumor-Detection
1-Dataset Creation:
The data includes two numerical features: File Count and Description_Length, and a target Subdirectory that is encoded into 0 (no tumor) and 1 (tumor).

2-Train-Test Split:
The data is split into 67% training and 33% testing, using stratify=y to ensure balanced classes in both training and testing datasets.

3-Model Training:
Random Forest Model: A RandomForestClassifier with 100 trees is trained on the data.
Decision Tree Model: A simpler DecisionTreeClassifier with a maximum depth of 3 is also trained.

4-Prediction and Evaluation:
Predictions are made on the test data using both models.
The accuracy and classification report (which includes precision, recall, f1-score) are printed for both models. 
