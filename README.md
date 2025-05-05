# 🧠 Breast Cancer Detection using Support Vector Machines (SVM)

## 📌 Objective
Use Support Vector Machines (SVM) with linear and RBF kernels to classify tumors as **malignant** or **benign** using the Breast Cancer Wisconsin (Diagnostic) Dataset.

---

## 📂 Dataset
**Path**: `/content/breast-cancer.csv`  
The dataset includes features derived from breast mass cell nuclei images, and the target column (`diagnosis`) indicates:
- `M` → Malignant (encoded as 1)
- `B` → Benign (encoded as 0)

---

## 🛠️ Tools & Libraries
- Python 3
- NumPy
- Pandas
- Scikit-learn
- Matplotlib
- Seaborn (optional)

---

## 🚀 Steps Performed

1. **Data Loading & Preprocessing**
   - Loaded the CSV file using Pandas
   - Dropped unnecessary columns (e.g., ID or unnamed columns)
   - Converted diagnosis labels to binary (M → 1, B → 0)
   - Normalized features using StandardScaler

2. **Model Training**
   - Trained two SVM models:
     - Linear kernel
     - RBF kernel

3. **Visualization**
   - Used PCA to reduce dimensionality to 2D
   - Plotted decision boundary

4. **Hyperparameter Tuning**
   - Used `GridSearchCV` to tune `C` and `gamma` parameters

5. **Evaluation**
   - Performed 5-fold cross-validation
   - Final output:
     ```
     Cross-validation accuracy: 0.98 (+/- 0.01)
     ```

---

## 📊 Results
- **Best Model**: RBF SVM with optimal `C` and `gamma`
- **Cross-validation Accuracy**: 98%
- **Low Variance**: ±1%, indicating high reliability
- **Conclusion**: SVM performs excellently on this medical diagnosis task



