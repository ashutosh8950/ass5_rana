---

# 🧠 Random Forest Optimization on UCI Wine Quality Dataset

This project focuses on optimizing a **Random Forest** classifier on the UCI **Wine Quality Dataset**. The goal is to improve classification performance through parameter tuning across multiple randomized splits.

---

## 📊 Dataset Overview

- **Source:** [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/wine+quality)
- **Type:** Multi-class classification (wine quality score: 0–10)
- **Size Used:** 5,000 rows (random subset from red and white wine combined)

---

## 🧪 Project Steps

1. 🔽 **Load and preprocess** dataset  
2. 🔄 **Generate 10 different 70/30 train-test splits**  
3. 🔧 **Optimize Random Forest** parameters:
   - `n_estimators`: 50, 100, 150  
   - `max_depth`: 5, 10, None  
   - `criterion`: `gini`, `entropy`  
   - 20 random parameter combinations per split  
4. 📈 **Track accuracy** of each configuration  
5. 🥇 **Identify best hyperparameters** and **visualize convergence** for the top-performing run

---

## 📌 Results Summary

| Sample | Best Accuracy | n_estimators | max_depth | Criterion |
|--------|----------------|--------------|-----------|-----------|
| S1     | 0.8320         | 100          | 10        | gini      |
| S2     | 0.8410         | 150          | None      | entropy   |
| S3     | **0.8530**     | 150          | None      | gini      |
| S4     | 0.8370         | 100          | 10        | entropy   |
| S5     | 0.8400         | 100          | 10        | gini      |
| S6     | 0.8330         | 150          | None      | entropy   |
| S7     | 0.8450         | 150          | None      | gini      |
| S8     | 0.8310         | 100          | 10        | entropy   |
| S9     | 0.8390         | 150          | 10        | gini      |
| S10    | 0.8470         | 150          | None      | gini      |

✅ Best accuracy achieved: **85.30% (S3)**

---

## 📊 Convergence Plot (S3)

![convergence_plot_s3](https://github.com/user-attachments/assets/convergence_plot_s3.png)

---

## 🛠️ Tech Stack

- Python  
- scikit-learn  
- pandas, numpy  
- matplotlib, seaborn  

---

## 💾 How to Run

```bash
pip install -r requirements.txt
python random_forest_optimizer.py
```

---

## License
This project is licensed under the MIT License.

---

## 📬 Contact
For queries, reach out to **Ashutosh Gupta** at [guptaashutosh8950@gmail.com].

---
