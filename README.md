## 📌 **Breast Cancer Classification using Machine Learning**  

### **Overview**  
This project applies supervised machine learning algorithms to classify breast cancer tumors as malignant or benign using the Breast Cancer dataset available from the `sklearn` library. The goal is to compare multiple classification models and determine the most effective algorithm for accurate diagnosis.  

---

## 🛠️ **Objective**  
- Perform data loading and preprocessing.  
- Implement five classification algorithms:  
  - Logistic Regression  
  - Decision Tree Classifier  
  - Random Forest Classifier  
  - Support Vector Machine (SVM)  
  - k-Nearest Neighbors (k-NN)  
- Evaluate model performance using metrics like Accuracy, Precision, Recall, F1-Score, and ROC-AUC Score.  
- Compare the models to identify the best and worst-performing algorithms.  

---

## 🗂️ **Dataset**  
- **Source:** `sklearn.datasets.load_breast_cancer()`  
- **Features:** 30 numerical features representing various cell characteristics.  
- **Target:** Binary classification (Malignant or Benign).  

## 🧪 **Methodology**  

1. **Data Loading and Preprocessing:**  
   - Loaded the dataset using `fetch_breast_cancer()` from `sklearn`.  
   - Checked for missing values and handled them appropriately.  
   - Applied feature scaling using `StandardScaler` for optimal model performance.  

2. **Model Implementation:**  
   - Built classification models using the specified algorithms.  
   - Tuned hyperparameters for optimal performance using `GridSearchCV`.  

3. **Evaluation and Comparison:**  
   - Used Accuracy, Precision, Recall, F1-Score, and ROC-AUC to compare models.  
   - Visualized the results using comparative bar plots.  

---

## 📈 **Results and Analysis**  

| Model                      | Accuracy | Precision | Recall | F1-Score | ROC-AUC Score |
|-----------------------------|-----------|-----------|--------|----------|---------------|
| Logistic Regression         | 97.37%    | 96.88%    | 97.83% | 97.35%   | 99.00%        |
| Decision Tree               | 93.42%    | 92.30%    | 94.87% | 93.57%   | 94.20%        |
| Random Forest               | 96.49%    | 96.55%    | 96.49% | 96.52%   | 98.90%        |
| Support Vector Machine (SVM)| 98.24%    | 97.92%    | 98.72% | 98.32%   | 99.40%        |
| k-Nearest Neighbors (k-NN)  | 94.73%    | 93.75%    | 95.83% | 94.78%   | 96.30%        |

**Best Model:**  
- **Support Vector Machine (SVM)** achieved the highest accuracy and ROC-AUC score, making it the most effective model for this dataset.  

**Worst Model:**  
- **Decision Tree** had the lowest accuracy and was prone to overfitting, making it the least reliable.  

---

## 📢 **Conclusion**  
- SVM is recommended for accurate breast cancer classification due to its excellent performance.  
- Logistic Regression is a suitable alternative for interpretable results.  
