Here is your **GitHub-ready `README.md`** content 👇
You can directly copy this into a `README.md` file.

---

# 🧪 Inferential Statistics on Healthcare Dataset

### 📊 Hypothesis Testing | Confidence Intervals | ANOVA | Correlation Analysis

> A complete statistical analysis project using Python to apply inferential statistics techniques on real-world healthcare data.

---

## 📌 Project Overview

This project demonstrates the practical implementation of **Inferential Statistics** concepts using a healthcare dataset.

It covers:

* Hypothesis formulation
* Confidence Interval estimation
* t-test
* Chi-square test
* ANOVA
* Covariance & Correlation
* Statistical Interpretation

The objective is to draw meaningful conclusions from sample data and interpret statistical test results scientifically.

---

## 🎯 Objectives

✔ Understand Inferential Statistics
✔ Perform Hypothesis Testing
✔ Compare group means using t-test
✔ Analyze categorical association using Chi-Square
✔ Perform ANOVA across multiple groups
✔ Measure correlation between variables
✔ Interpret statistical results clearly

---

## 📂 Dataset Used

**File:** `health_records.csv`

The dataset includes variables such as:

* `age`
* `weight`
* `bmi`
* `cholesterol_level`
* `diabetes` (True/False)
* `smoking_status`
* `age_group`

---

## 🛠️ Technologies & Libraries

```python
pandas
numpy
scipy
math
matplotlib
```

---

# 📘 Project Breakdown

---

## 🧠 Part A – Theoretical Foundation

### 🔹 What is Inferential Statistics?

Inferential statistics allows us to:

* Make predictions about a population
* Test hypotheses
* Estimate population parameters
* Determine relationships between variables

---

# 📊 Part B – Data Analysis & Testing

---

## 1️⃣ Hypothesis Formulation

### 🔹 Hypothesis 1: Smoking vs Diabetes

* **H₀:** Smoking has no effect on diabetes
* **H₁:** Smoking affects diabetes

### 🔹 Hypothesis 2: Cholesterol vs Diabetes

* **H₀:** Mean cholesterol levels are equal
* **H₁:** Mean cholesterol levels are different

---

## 2️⃣ Confidence Intervals (95%)

Calculated manually using:

[
CI = \bar{x} \pm Z \times \frac{s}{\sqrt{n}}
]

Confidence intervals were computed for:

* Age
* Weight
* BMI

This helps estimate the range in which the population mean lies with 95% confidence.

---

## 3️⃣ t-Test (Independent Samples)

Used to compare cholesterol levels between:

* Diabetic patients
* Non-diabetic patients

```python
stats.ttest_ind(diabetes_yes, diabetes_no)
```

### 📌 Interpretation

If `p-value < 0.05` → Reject H₀
If `p-value ≥ 0.05` → Accept H₀

✔ In this project:
**Cholesterol levels differ significantly between diabetic and non-diabetic patients.**

---

## 4️⃣ Chi-Square Test

Used to determine association between:

* Smoking Status
* Diabetes

Steps:

* Create contingency table
* Calculate expected values
* Compute Chi-square statistic

### 📌 Conclusion

If p-value < 0.05 → Significant association exists.

---

## 5️⃣ ANOVA (Analysis of Variance)

Used to compare BMI across different age groups.

```python
stats.f_oneway(*groups)
```

### 📌 Interpretation

* Tests whether at least one group mean differs
* If p-value < 0.05 → Significant difference exists

---

## 6️⃣ Covariance & Correlation

Examined relationship between:

* Age
* Cholesterol Level

### 🔹 Manual Covariance Calculation

[
Cov(X,Y) = \frac{\sum (X - \bar{X})(Y - \bar{Y})}{n-1}
]

### 🔹 Spearman Correlation

```python
spearmanr(X, Y)
```

---

## 📈 Visualization

A scatter/line plot was created:

* **Age vs Cholesterol Level**

This helps visually inspect trends and relationships between variables.

---

# 🧾 Final Results Summary

| Test        | Result                 | Decision                       |
| ----------- | ---------------------- | ------------------------------ |
| t-test      | p-value < 0.05         | Reject H₀                      |
| Chi-square  | Based on p-value       | Association checked            |
| ANOVA       | F-statistic computed   | Group comparison               |
| Correlation | Coefficient calculated | Relationship strength measured |

---

# 📊 Key Learnings

✅ Manual vs Built-in statistical computation
✅ Difference between Z-test & t-test
✅ Hypothesis testing workflow
✅ Statistical interpretation in real-world context
✅ Data-driven decision making

---

# 🚀 How to Run the Project

1. Clone the repository

```bash
git clone https://github.com/your-username/your-repo-name.git
```

2. Install dependencies

```bash
pip install pandas numpy scipy matplotlib
```

3. Open the notebook

```bash
jupyter notebook pr3.ipynb
```

4. Run all cells sequentially

---

# 📁 Project Structure

```
📦 Inferential-Statistics-Healthcare
 ┣ 📜 pr3.ipynb
 ┣ 📊 health_records.csv
 ┗ 📄 README.md
```

---

# 💡 Future Improvements

* Add regression analysis
* Include more visualizations
* Build a dashboard using Streamlit
* Automate report generation

---

# 👨‍💻 Author

**Dharmik Pansuriya**
📊 Data Analytics & Machine Learning Enthusiast

---

# ⭐ If You Like This Project

Give it a ⭐ on GitHub and share it with others!

---

🔥 *This project demonstrates the practical power of statistics in solving real-world healthcare problems.*
