🫀 Heart Disease Prediction using Machine Learning
This project predicts the likelihood of heart disease based on patient data using various machine learning models, including a highly accurate Random Forest Classifier. The implementation is done in Python using Google Colab.

 📁 Dataset

File: `heart.csv`
Contains medical features such as:

 `age`, `sex`, `cp` (chest pain type), `trestbps` (resting blood pressure), `chol` (cholesterol), `fbs` (fasting blood sugar), etc.
 Target variable: `target` (1 = heart disease, 0 = no heart disease)

 ✅ Requirements
Install these in your Colab notebook (already pre-installed in most cases):
bash
!pip install scikit-learn matplotlib graphviz


📌 Steps Performed
1. Data Loading

 Upload `heart.csv` manually using:
    python
     from google.colab import files
     uploaded = files.upload()
    

2. Data Preprocessing
   Checked missing values, understood feature distribution

3. Splitting the Dataset

   ```python
   from sklearn.model_selection import train_test_split
   X = df.drop("target", axis=1)
   y = df["target"]
   X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)

4. Model Training

     * Trained multiple models, including
     * Decision Tree
     * Random Forest (Best Accuracy: 99%)

5. Evaluation

   * Accuracy
   * Cross-validation score
