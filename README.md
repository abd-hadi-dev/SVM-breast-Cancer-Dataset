# Breast Cancer Classification using Support Vector Machines (SVM)

This project applies Support Vector Machines (SVM) to classify breast tumors as benign or malignant using medical imaging features. Both linear and non-linear SVM models are explored to understand how they perform on this classification task.

---

## 📌 Objective

To build a machine learning model that accurately distinguishes between malignant and benign breast tumors using SVM classifiers with different kernels.

---

## 📊 Dataset Description

The dataset consists of various numerical features extracted from breast mass images. Each row corresponds to one tumor instance.

- **Number of features:** 30 (e.g., texture, symmetry, compactness)
- **Target labels:**
  - `1`: Malignant
  - `0`: Benign

### Preprocessing Steps

- Dropped unnecessary identifiers
- Converted diagnosis labels to binary
- Standardized features to mean 0 and variance 1

---

## 📁 Project Files

| File Name                | Purpose                                                 |
|--------------------------|---------------------------------------------------------|
| `svm_breast_cancer.ipynb`| Main code notebook with preprocessing, training, and plots |
| `data.csv`               | Cleaned dataset used for training and evaluation        |
| `pca_visualization.png`  | 2D PCA plot showing class separation                    |
| `README.md`              | Project description and usage guide                     |

---

## 🔧 Model Implementation

Two types of SVM models were trained:

- **Linear SVM:** for detecting simple linear separations
- **RBF SVM:** for capturing more complex, non-linear relationships

Hyperparameter tuning was done using Grid Search to find the best combination of `C` and `gamma` values. Cross-validation (5-fold) ensured the model's performance was reliable.

---

## 📈 Visualization

Principal Component Analysis (PCA) was applied to reduce dimensions to 2D, allowing the decision boundaries to be visualized and compared between models.

---

## 🔍 Key Findings

- **RBF SVM outperformed** linear SVM by handling non-linear patterns better
- **Standardization** greatly improved model accuracy
- **Cross-validation** helped ensure consistent results across different splits

---

## ▶️ How to Run the Code

1. Open the project notebook in [Google Colab](https://colab.research.google.com/)
2. Upload the `data.csv` file
3. Run all cells to:
   - Preprocess the data
   - Train both SVM models
   - Visualize decision boundaries
4. Review classification reports and accuracy

---

## ✅ Tools Used

- Python
- Scikit-learn
- NumPy & Pandas
- Matplotlib & Seaborn
- Google Colab

---

## 📬 Contact

If you have any questions or suggestions, feel free to open an issue on this repository.

