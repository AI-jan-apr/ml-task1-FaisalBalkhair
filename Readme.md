[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/3TS0mELD)

# Model Interpretation & Discussion

## 1. Overall Performance

All three models achieved high performance on the Breast Cancer dataset.  
This suggests that the dataset is well-structured and largely linearly separable.

Among the three models, **Logistic Regression** achieved the best overall performance based on Accuracy and F1-score.  
SVM performed very similarly, while KNN showed slightly lower performance compared to the other two models.

---

## 2. Why Did Logistic Regression Perform Well?

The Breast Cancer dataset contains numerical features with strong linear relationships to the target variable.  
Since Logistic Regression is a linear classifier, it performs well when the data is close to linearly separable.

Additionally:

- No missing values
- Balanced class distribution
- Clean numerical features

These factors contribute to strong performance for linear models.

---

## 3. Medical Context Interpretation

In a medical diagnosis setting, **Recall is the most important metric**.

Recall measures:

> Out of all actual malignant (cancerous) tumors, how many were correctly identified?

A False Negative (predicting a malignant tumor as benign) can be life-threatening.  
Therefore, minimizing False Negatives is critical.

In this case, all models achieved very high Recall, which makes them suitable for medical screening purposes.

---

## 4. Model Recommendation

Although all models performed well, **Logistic Regression** is recommended because:

- It achieved the best overall balance of metrics.
- It provides high Recall.
- It is more interpretable compared to SVM and KNN.

Model interpretability is especially important in healthcare applications.

---

## 5. Limitations

- No hyperparameter tuning was performed.
- Feature scaling was not used (as required by the task).
- Cross-validation was not applied.
- Performance might change with further optimization.

---

# Final Conclusion

Logistic Regression performed best overall among the three models.  
In a medical context, Recall is the most critical metric because failing to detect a malignant tumor can have serious consequences.
