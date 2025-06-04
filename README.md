# ai-ml_intern-Task-5
This project uses tree-based models to predict heart disease using the `heart.csv` dataset. The models implemented include a **Decision Tree Classifier** and a **Random Forest Classifier**, with visualization and evaluation.
## 📂 Dataset

- **File**: `heart.csv`
- **Target**: `target` (1 = disease, 0 = no disease)
- Features include:
  - `age`, `sex`, `cp` (chest pain), `trestbps` (resting BP), `chol` (cholesterol),
  - `thalach` (max heart rate), `oldpeak`, `thal`, etc.

---
![Screenshot 2025-06-04 103923](https://github.com/user-attachments/assets/309faa79-425c-4249-9a58-dd1f314dc5ab)


## 🛠️ Tools & Libraries

- Python, Scikit-learn, Matplotlib, Seaborn
- Optional: Graphviz for advanced visualization

---

## 🚀 Steps

### 1. Train a Decision Tree Classifier
- Use `DecisionTreeClassifier` from `sklearn`.
- Visualize the decision tree using `plot_tree`.
- ![Screenshot 2025-06-04 103952](https://github.com/user-attachments/assets/4c9e10cb-a41f-47d6-8406-c012054a7119)


### 2. Analyze Overfitting
- Vary `max_depth` from 1 to 20.
- Plot training vs. test accuracy to observe bias-variance tradeoff.
- ![Screenshot 2025-06-04 104007](https://github.com/user-attachments/assets/b98011b9-7606-4c9b-88f3-ac0b8c61380f)


### 3. Train a Random Forest
- Use `RandomForestClassifier` with default or tuned hyperparameters.
- Compare accuracy with Decision Tree.

Decision Tree Accuracy: 0.9707792207792207
Random Forest Accuracy: 0.9805194805194806

### 4. Interpret Feature Importances
- Use `feature_importances_` from the Random Forest.
- Visualize using a bar chart.
![image](https://github.com/user-attachments/assets/4d835217-2cec-4c15-8c4e-1862d6229831)

### 5. Evaluate Using Cross-Validation
- Apply `cross_val_score` for a more robust accuracy estimate.
- Report mean ± standard deviation.

---Random Forest CV Accuracy: 0.997 ± 0.006

## 📊 Results

- **Decision Tree Accuracy**: ~ Decision Tree Accuracy: 0.9707792207792207
- **Random Forest Accuracy**: Random Forest Accuracy: 0.9805194805194806
- **Important Features**: `thalach`, `oldpeak`, `cp`, etc. (depends on model output)

---

## ✅ Requirements

```bash
pip install pandas scikit-learn matplotlib seaborn
📁 File Structure
Copy
Edit
├── heart.csv
├── decision_tree_random_forest.ipynb
├── README.md
