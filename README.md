# Support Vector Machine (SVM) and Hyperparameter Tuning with GridSearchCV

## 📌 What is Support Vector Machine (SVM)?
Support Vector Machine (SVM) is a **supervised machine learning algorithm** used for **classification** and **regression** tasks. It works by finding the best possible decision boundary (hyperplane) that separates different classes.

### 🎯 Key Concepts of SVM:
1. **Hyperplane**: A decision boundary that separates different classes.
2. **Support Vectors**: The closest data points to the hyperplane that influence its position.
3. **Margin**: The distance between the hyperplane and the nearest support vectors. SVM aims to maximize this margin.
4. **Kernel Trick**: Transforms data into a higher dimension to make it separable.

## ⚙️ Types of SVM:
- **Linear SVM**: Works well when data is linearly separable.
- **Non-Linear SVM**: Uses kernel functions to classify complex datasets.

## 🔧 Important Hyperparameters of SVM:
1. **C (Regularization Parameter)**: Controls the trade-off between achieving a low error and having a large margin.
   - High **C** → More focus on classifying points correctly (less margin).
   - Low **C** → More focus on a larger margin (can tolerate some misclassification).
2. **Kernel Function**: Defines how data is transformed. Common kernels include:
   - `'linear'` (Linear Kernel)
   - `'rbf'` (Radial Basis Function)
   - `'poly'` (Polynomial Kernel)
3. **Gamma (For RBF Kernel)**: Controls how much influence a single training point has.
   - High **gamma** → Points closer to the decision boundary have more influence.
   - Low **gamma** → Points farther away also contribute.

## 🔍 Hyperparameter Tuning with GridSearchCV
`GridSearchCV` helps find the best combination of hyperparameters using **cross-validation**.

### Steps to Perform Hyperparameter Tuning:
1. Define the **parameter grid** (list of hyperparameter values to try).
2. Use `GridSearchCV` to test all possible combinations.
3. Select the best combination based on performance.


##  Summary
- SVM is a powerful classifier that finds the optimal decision boundary.
- Key hyperparameters include **C**, **kernel**, and **gamma**.
- `GridSearchCV` automates the process of finding the best hyperparameters.
- Using proper tuning can significantly **improve model performance**.
