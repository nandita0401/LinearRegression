# 📈 Linear Regression — Student Score Predictor

![Language](https://img.shields.io/badge/Language-Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Library](https://img.shields.io/badge/Library-Scikit--Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Tool](https://img.shields.io/badge/Tool-Jupyter%20Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)

> A supervised machine learning project that uses Simple Linear Regression to predict a student's exam score percentage based on the number of hours they studied — with model training, visualization, and error evaluation.

---

## 📖 Table of Contents

- [About the Project](#about-the-project)
- [Problem Statement](#problem-statement)
- [How It Works](#how-it-works)
- [Tech Stack](#tech-stack)
- [Model Performance](#model-performance)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Project Structure](#project-structure)
- [Sample Output](#sample-output)
- [Future Improvements](#future-improvements)
- [Author](#author)

---

## About the Project

This project demonstrates a foundational machine learning pipeline from **data loading → visualization → model training → prediction → evaluation**. It applies **Simple Linear Regression** using Scikit-Learn to model the relationship between study hours and student exam performance.

Despite its simplicity, this project showcases the complete workflow that underpins all supervised ML projects — making it a solid demonstration of core ML engineering skills.

---

## Problem Statement

> **Given the number of hours a student studies, predict the percentage score they are likely to achieve in an exam.**

This is a classic **supervised regression** problem with:
- **Input (X):** Hours studied
- **Output (y):** Exam score percentage

---

## How It Works
```
1. Load Dataset
   └── Read student scores CSV from remote URL (Pandas)

2. Explore & Visualize
   └── Scatter plot of Hours vs Score to confirm linear relationship

3. Prepare Data
   └── Split features (X) and labels (y)
   └── Train/Test split — 80% training, 20% testing (random_state=0)

4. Train Model
   └── Fit LinearRegression model on training data (Scikit-Learn)

5. Visualize Regression Line
   └── Plot fitted regression line over scatter data

6. Predict & Evaluate
   └── Predict scores on test set
   └── Compare Actual vs Predicted values
   └── Calculate Mean Absolute Error (MAE)
```

---

## Tech Stack

| Tool | Purpose |
|---|---|
| Python 3.x | Core programming language |
| Pandas | Data loading and manipulation |
| NumPy | Numerical operations |
| Matplotlib | Data visualization and regression line plotting |
| Scikit-Learn | Model training, train/test split, MAE evaluation |
| Jupyter Notebook | Interactive development environment |

---

## Model Performance

The model is evaluated using **Mean Absolute Error (MAE)** — the average absolute difference between actual and predicted scores:

| Metric | Value |
|---|---|
| Algorithm | Simple Linear Regression |
| Train/Test Split | 80% / 20% |
| Evaluation Metric | Mean Absolute Error (MAE) |

> 📝 Update this table with your actual MAE value after running the notebook.

---

## Getting Started

### Prerequisites
```bash
pip install pandas numpy matplotlib scikit-learn jupyter
```

### Installation

1. **Clone the repository**
```bash
   git clone https://github.com/nandita0401/LinearRegression.git
   cd LinearRegression
```

2. **Launch Jupyter Notebook**
```bash
   jupyter notebook
```

3. **Open and run the file**
```
   Open LinearRegression.txt (or rename to .ipynb)
   Run → Restart & Run All
```

> 💡 **Tip:** Rename `LinearRegression.txt` to `LinearRegression.ipynb` for proper Jupyter rendering with cell outputs and inline plots.

---

## Project Structure
```
LinearRegression/
├── LinearRegression.txt    # Python source code (rename to .ipynb for Jupyter)
└── README.md
```

---

## Sample Output

**Actual vs Predicted Scores:**

| Hours Studied | Actual Score | Predicted Score |
|---|---|---|
| 1.5 | 20 | ~17 |
| 3.2 | 27 | ~31 |
| 7.4 | 69 | ~75 |
| 9.0 | 88 | ~92 |

> 📝 Replace these with your actual output values from the notebook.

**Visualizations produced:**
- Scatter plot of Hours vs Percentage Score
- Regression line fitted over the full dataset

---

## Future Improvements

- [ ] Rename `.txt` to `.ipynb` for proper Jupyter Notebook rendering
- [ ] Add **R² score** alongside MAE for a more complete evaluation
- [ ] Extend to **Multiple Linear Regression** with additional features (attendance, sleep hours, etc.)
- [ ] Build a simple **prediction UI** using Streamlit — input study hours, get predicted score
- [ ] Add **cross-validation** for more robust model evaluation

---

## Author

**Nandita Bharambe**

[![GitHub](https://img.shields.io/badge/GitHub-nandita0401-181717?style=flat&logo=github)](https://github.com/nandita0401)

---

> 💡 *This project demonstrates the end-to-end machine learning workflow — from raw data to a trained, evaluated model. Every complex ML system is built on these same foundational steps.*
