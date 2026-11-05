# Sleep-Disorder-Prediction
Machine learning project that predicts Insomnia, Sleep Apnea, or No Disorder based on sleep patterns and lifestyle habits. Compares Decision Tree and Random Forest algorithms to identify the best-performing model.

---

## 📌 Project Overview

Sleep is essential for a healthy life, yet many people experience sleep disorders without recognizing the warning signs. This project uses machine learning to analyze sleep patterns and lifestyle habits to predict possible sleep disorders, helping identify risks early and promote better sleep health.

Two classification algorithms, Decision Tree and Random Forest, are trained and compared to find the most accurate model.

---

## 🎯 Objectives

- To analyze sleep patterns and lifestyle factors.
- To identify the best-performing prediction model.

---

## ✨ Features

- Works on a dataset of **1,200 records** with **13 features**.
- Predicts one of three categories: **Insomnia**, **Sleep Apnea**, or **No Disorder**.
- Includes data preprocessing, encoding, and feature scaling.
- Compares two algorithms using Accuracy, Precision, Recall, F1-Score, and Macro F1-Score.
- Includes a confusion matrix and a model comparison graph.

### Dataset Summary

| Item | Details |
| --- | --- |
| Total records | 1,200 |
| Total features | 13 |
| Target variable | Sleep Disorder |
| Categories | Insomnia, Sleep Apnea, No Disorder |
| Train / Test split | 960 / 240 (80:20) |

---

## 🤖 Machine Learning

### Algorithms Used

| Algorithm | Purpose |
| --- | --- |
| Decision Tree | Predicts outcomes using decision-based splits |
| Random Forest | Combines multiple decision trees and uses majority voting |

### Evaluation Metrics

- **Accuracy:** measures overall correct predictions.
- **Precision:** measures correctness of positive predictions.
- **Recall:** measures correctly identified actual cases.
- **F1-Score:** balances precision and recall.
- **Macro F1-Score:** treats all classes equally.

### Results

| Metric | Decision Tree | Random Forest |
| --- | --- | --- |
| Accuracy | 47.50% | **56.25%** |
| Precision | 31.57% | **35.43%** |
| Recall | 31.32% | **35.35%** |
| F1-Score | 31.30% | **35.32%** |

### 🏆 Best Algorithm: Random Forest

- Achieved higher accuracy than Decision Tree.
- Classifies all three sleep disorder categories more effectively.
- Combines multiple decision trees for stable predictions.

### Graph Insights

- **Confusion Matrix:** Random Forest correctly predicts 123 No Disorder, 4 Insomnia, and 8 Sleep Apnea cases.
- **Model Comparison:** Random Forest outperforms Decision Tree with higher accuracy (56.25%) and Macro F1-score (35.32%).

---

## 🛠️ Technologies Used

| Category | Tools |
| --- | --- |
| Language | Python |
| Libraries | Pandas, NumPy, Scikit-learn |
| Visualization | Matplotlib, Seaborn |
| Environment | Jupyter Notebook / Google Colab |
| Version control | Git and GitHub |

---

## 📁 Project Structure

```
sleep-disorder-prediction/
├── README.md                          # Project documentation
├── requirements.txt                   # Python dependencies
├── data/
│   └── sleep_disorder_dataset.csv     # Dataset (1,200 records, 13 features)
├── notebooks/
│   └── sleep_disorder_prediction.ipynb  # Complete code
├── results/
│   ├── confusion_matrix.png           # Random Forest confusion matrix
│   └── model_comparison.png           # Decision Tree vs Random Forest
└── docs/
    └── Case_Study_Slides.pptx         # Presentation
```

---

## 🔄 Machine Learning Workflow

1. **Data collection:** load the sleep dataset (1,200 records, 13 features).
2. **Data preprocessing:** clean the data and handle missing values.
3. **Encoding:** convert categorical columns into numeric form.
4. **Feature scaling:** scale the features.
5. **Train–test split:** 80:20 split, giving 960 training and 240 testing records.
6. **Model training:** train Decision Tree and Random Forest.
7. **Model testing:** predict sleep disorder on the 240 test records.
8. **Evaluation:** calculate Accuracy, Precision, Recall, F1-Score, and Macro F1-Score, and plot the confusion matrix.
9. **Model comparison:** compare both models.
10. **Best model selection:** choose Random Forest, which has the higher accuracy and Macro F1-score.

---

## ▶️ How to Run

```bash
git clone https://github.com/<your-username>/sleep-disorder-prediction.git
cd sleep-disorder-prediction
pip install -r requirements.txt
jupyter notebook notebooks/sleep_disorder_prediction.ipynb
```

---

## 🚀 Future Enhancements

- Improve accuracy with more data and better feature selection.
- Handle class imbalance, since most records fall under No Disorder.
- Apply hyperparameter tuning (for example GridSearchCV) to both models.
- Try more models such as XGBoost, SVM, or deep learning.
- Build a web app where a user enters sleep and lifestyle details and gets a predicted risk.

---

## 📊 Project Status

**Completed**: model training, evaluation, comparison, and result visualization are done. The project is open to the enhancements listed above.

---

## 💡 Conclusion

Healthy sleep habits and lifestyle choices play an important role in maintaining overall well-being and reducing the risk of sleep disorders. Proper sleep, stress management, and regular physical activity contribute to better sleep quality, improved daily performance, and a healthier life.

---

