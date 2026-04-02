Handwritten Digit Recognition using SVM
📌 Project Overview

This project focuses on recognizing handwritten digits (0–9) using a Support Vector Machine (SVM) model. It uses a built-in dataset from Scikit-learn and demonstrates image processing, model training, and evaluation.

🎯 Objective

To build a machine learning model that can correctly identify handwritten digits based on pixel values.

🛠️ Technologies Used
Python 
NumPy
Matplotlib
Scikit-learn
 Dataset
Dataset used: Digits Dataset (from sklearn)
Total samples: 1797 images
Each image size: 8 × 8 pixels
Classes: Digits from 0 to 9
⚙️ Steps Performed
1. Import Libraries

Essential libraries for data handling and visualization.

2. Load Dataset

Dataset is loaded using:

from sklearn.datasets import load_digits
dataset = load_digits()
3. Data Exploration
Checked dataset structure
Viewed image data and labels
Total number of images: 1797
4. Data Visualization

Displayed sample digit image using Matplotlib.

5. Data Preprocessing
Images reshaped from 2D (8×8) → 1D (64 features)
Prepared input (X) and output (Y)
6. Train-Test Split

Dataset split into:

75% Training data
25% Testing data
7. Model Training

Used Support Vector Machine (SVM):

from sklearn import svm
model = svm.SVC(kernel='linear')
model.fit(X_train, y_train)
8. Prediction
Predicted digit from test images
Displayed predicted digit with image
9. Model Evaluation

Accuracy calculated using:

from sklearn.metrics import accuracy_score
10. Model Comparison

Tested different SVM models:

Linear Kernel
RBF Kernel
Gamma tuning
C parameter tuning
📊 Sample Output
Predicted Digit: 5
Accuracy of the Model: 97%

(Accuracy may vary depending on parameters)

 How to Run
Open in Google Colab / Jupyter Notebook
Run all cells step by step
View predictions and accuracy
💡 Example Visualization
Displays handwritten digit image
Shows predicted output
🚀 Future Improvements
Use deep learning (CNN)
Improve accuracy with hyperparameter tuning
Deploy as a web application
Use custom handwritten datasets
👨‍💻 Author
fathimath zuhra
