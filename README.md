# MNIST Generalization Study  
### Overfitting vs Regularization in Deep Learning (PyTorch)

---

> A focused study on generalization in deep learning

> Demonstrating overfitting and regularization dynamics on MNIST.


## 📌 Overview

This project explores **model generalization** by intentionally:

- Creating an overfitting model
- Applying regularization techniques
- Comparing training vs validation behavior

The goal is to understand how deep networks memorize vs generalize.

---

## 🎯 Objectives

1. Build a strong baseline CNN
2. Force overfitting on MNIST
3. Reduce generalization gap using regularization
4. Analyze training dynamics

---

## 🧠 Key Learnings

- High-capacity models easily memorize data
- Overfitting appears as a growing train–val gap
- Regularization improves generalization
- Data augmentation acts as implicit regularization

---

## 🛠 Tech Stack

- PyTorch
- Torchvision
- NumPy
- Matplotlib

---

## 📂 Project Structure

src/ → training scripts

results/ → plots and logs

notebooks/ → experiments


---

## 📊 Experiments

### Task 1 — Baseline CNN
- Standard CNN
- Good generalization
- Small train–val gap

### Task 2 — Overfitting
- Large MLP
- No dropout
- High capacity
- Gap > 2%

### Task 3 — Regularization
Applied:

- Dropout
- Weight decay
- Label smoothing
- Data augmentation
- LR scheduling

Result:

✅ Gap < 0.5%  
✅ Stable validation accuracy

---

## 📈 Results

### Overfitting Curve
![Overfitting](results/task2_curves.png)

### Regularized Curve
![Regularized](results/task3_curves.png)

---

## 🚀 How to Run

pip install -r requirements.txt 

python src/task1_baseline.py

python src/task2_overfit.py

python src/task3_regularized.py


---

## 📌 Future Work

- Try CIFAR-10
- Explore Mixup/CutMix
- Study double descent

---

## 👤 Author

Manikanta Koushik  
AI/ML Student & Research Intern
