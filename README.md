# KNN Breast Cancer Classifier

![Python](https://img.shields.io/badge/Python-3.10+-blue) ![sklearn](https://img.shields.io/badge/scikit--learn-KNN-orange)

KNN classification on the Wisconsin Breast Cancer dataset. Covers feature scaling, hyperparameter tuning, clinical metric analysis, and feature reduction.


---

## Tasks

| # | Topic | Key Finding |
|---|-------|-------------|
| 1 | Feature Scaling | Unscaled KNN degrades — `StandardScaler` is mandatory |
| 2 | Hyperparameter Tuning | `weights='distance'` + Manhattan (`p=1`) optimises F1 |
| 3 | Clinical Priority | Recall > Precision for cancer screening; minimise False Negatives |
| 4 | Feature Importance | 2-feature model insufficient; retain full feature set |

---

## Results (Best K = 9)

| Metric | Score |
|--------|-------|
| Accuracy | 96.49% |
| Precision | 97.18% |
| Recall | 97.18% |
| F1-Score | 97.18% |
| AUC | 0.981 |


---

## 🛠 Dependencies

```bash
numpy pandas matplotlib seaborn scikit-learn jupyter
```

---

##  Dataset

- **Source:** `sklearn.datasets.load_breast_cancer`
- **Samples:** 569 &nbsp;|&nbsp; **Features:** 30 &nbsp;|&nbsp; **Classes:** Malignant (212) / Benign (357)
