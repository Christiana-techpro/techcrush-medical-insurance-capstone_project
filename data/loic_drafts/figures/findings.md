
### Summary of Univariate Findings

- **Target Variable (`charges`):**
  - Annual medical bills are heavily right-skewed, with a **median of $9,386** and a **mean of $13,279** pulled upward by a long right tail of claims extending past **$60,000**.
  - The density curve displays a **secondary bump between $35,000 and $48,000**, indicating that at least two distinct risk populations are mixed inside the dataset.
  - Boxplot outliers above roughly **$34,500** represent genuine high-cost medical claims rather than data-entry errors and must be retained for modeling.

- **Numeric Input Features (`age`, `bmi`, `children`):**
  - **`age`** spans 18 to 64 years and is distributed fairly evenly across adulthood, aside from a prominent spike at ages **18–19** with over 160 policyholders.
  - **`bmi`** follows a symmetric, bell-shaped (normal) distribution with a **mean of 30.7**, placing more than half of the customer base above the clinical obesity threshold of **30.0**.
  - **`children`** is strongly right-skewed.Over 570 policyholders have 0 dependents, while the 4- and 5-child groups each contain roughly 25 or fewer records, making them prone to small-sample noise.

- **Categorical Input Features (`smoker`, `sex`, `region`):**
  - **`smoker`** is imbalanced at roughly **80% non-smokers** (over 1,050 records) versus **20% smokers** (around 274 records), providing sufficient sample size in both groups for reliable comparison.
  - **`sex`** (nearly 50/50 female and male) and **`region`** (324–364 policyholders across southwest, southeast, northwest, and northeast) are evenly balanced across the portfolio.

### Hypotheses to Test in Step 2 (Bivariate Analysis)

1. **Primary Driver Hypothesis (`smoker` vs. `charges`):** The 20% smoker group explains the secondary $35,000–$48,000 cost peak in `charges` and incurs dramatically higher average bills than non-smokers.
2. **Age Progression Hypothesis (`age` vs. `charges`):** Annual medical bills rise steadily as `age` increases from 18 to 64, reflecting higher baseline healthcare utilization among older adults.
3. **Obesity Risk Hypothesis (`bmi` vs. `charges`):** Policyholders above the clinical obesity cutoff (BMI ≥ 30) incur higher annual medical costs, especially if obesity compounds the health risks of smoking.
4. **Low-Impact Feature Hypothesis (`sex`, `region`, `children` vs. `charges`):** Evenly balanced attributes like `sex` and `region`,along with `children`show minimal standalone effect on annual medical expenses.
