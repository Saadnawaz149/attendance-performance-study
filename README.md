# Attendance and Student Performance Analysis

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://githubtocolab.com/Saadnawaz149/attendance-performance-study/blob/main/final_project.ipynb)

## Author
**Saad Nawaz**  
Allegheny College — Computer Science  

---

## 📌 Project Overview

This project investigates how two key student engagement behaviors:

- **Class attendance**
- **Homework completion**

relate to overall **exam performance**.

Using a dataset of over **12,000 student records**, the analysis explores whether students who attend class consistently and submit homework regularly achieve higher exam scores.

---

## 🎯 Research Question

Do students with higher attendance rates and stronger homework completion perform better on exams?

---

## ✅ Hypothesis

Students who maintain higher attendance rates and more consistent homework completion will, on average, achieve higher exam scores than peers with lower engagement.

---

## 📊 Dataset Description

The dataset includes:

- Attendance logs (Present/Absent)
- Homework completion rates (mixed formats such as 80%, 0.75, etc.)
- Exam scores (numeric, with some outliers)
- Optional parent–teacher communication notes

The data was obtained from a CSV source on **Kaggle** and includes realistic inconsistencies such as missing values, formatting issues, and outliers.

---

## 🧹 Data Cleaning & Preprocessing

Several preprocessing steps were applied:

1. **Standardized attendance categories**
   - Converted inconsistent entries into clean `Present` or `Absent`

2. **Normalized date formats**
   - Parsed all date strings into a consistent structure

3. **Converted homework completion rates**
   - Removed `%` symbols and standardized all values into a 0–100 scale

4. **Cleaned exam scores**
   - Removed invalid values below 0 or above 100

5. **Handled missing data**
   - Dropped missing exam scores
   - Imputed missing attendance/homework entries when appropriate

6. **Aggregated to student-level metrics**
   - Attendance rate (%)
   - Average homework completion (%)
   - Average exam score

---

## 📈 Methods Used

The analysis includes:

- Descriptive statistics
- Histograms of attendance and homework completion
- Scatterplots comparing engagement vs. performance
- Pearson correlation
- Multiple linear regression modeling

---

## 🔍 Key Findings

- Students attended an average of **~80%** of classes  
- Homework completion averaged **~78%**  
- Mean exam score was approximately **75**

### Relationships Observed

- Higher attendance rates showed a **moderate positive association** with exam scores
- Homework completion displayed an even clearer upward trend with performance

Overall, engagement behaviors were strong predictors of student success.

---

## ⚠️ Limitations

- The dataset is partially synthetic and may not capture all real-world educational complexity  
- Observed relationships are **correlational**, not causal  
- Other factors (study habits, course difficulty, teacher effects) were not modeled  

---

## 📌 Conclusion

Both attendance and consistent homework completion are associated with better exam outcomes. This project reinforces the importance of regular participation and provides a reproducible pipeline for cleaning and analyzing educational performance data.

---

## 🛠 Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Jupyter Notebook

---

## 📂 Repository Contents

- `final_project.ipynb` — full analysis notebook  
- `.gitignore` — ignores system files  
- `README.md` — project documentation  

---

## 📚 Reference

Credé, M., Roch, S. G., & Kieszczynka, U. M. (2010).  
*Class attendance in college: A meta‐analytic review of the relationship of class attendance with grades and student characteristics.*  
Review of Educational Research, 80(2), 272–295.

---

## 🚀 How to Run

1. Clone this repository:

```bash
git clone https://github.com/Saadnawaz149/attendance-performance-study.git
