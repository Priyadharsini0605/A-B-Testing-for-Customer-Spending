# A/B Testing Analysis for Customer Spending

## Project Overview
This project explores customer spending behaviors across different experimental groups (A and B) to determine the significance of any differences. Using statistical methods like t-tests and post-hoc analysis, along with visualizations, this analysis evaluates the impact of group assignments and other variables like tenure and spending frequency.

---

## Results and Visualizations

### 1. Summary Statistics
#### Dataset Overview:
- **Number of entries**: 8950
- **Number of features**: 18
- **Missing Values**:
  - `CREDIT_LIMIT`: 1 missing value
  - `MINIMUM_PAYMENTS`: 313 missing values

#### Descriptive Statistics (Spending Columns):
- **Mean Spending**: 1003.20
- **Max Spending**: 49,039.57
- **Min Spending**: 0.0

---

### 2. Key Findings

#### a. T-Test Results
- **T-statistic**: -2.263
- **P-value**: 0.0236
- **Conclusion**: Reject the null hypothesis; there is a statistically significant difference in spending between Groups A and B.

#### b. Post-Hoc Analysis
Performed post-hoc analysis to identify subgroups contributing to the difference in spending based on tenure.
- Groups with **Long Tenure** showed higher spending compared to **Short Tenure**.

---

### 3. Visualizations

#### Spending Behavior Across Groups (A vs B)
- **Box Plot**:
  - Displays the spending distributions for Groups A and B.
  - Outliers observed in both groups, with Group B showing slightly higher spending on average.

#### Spending Distribution Across Groups
- **Histogram with KDE**:
  - Distribution is heavily right-skewed.
  - Group B shows marginally higher spending density at the higher end.

#### Spending by Tenure Group
- **Bar Plot**:
  - Customers with **Long Tenure** in Group B showed significantly higher spending compared to other subgroups.

#### Spending by Purchase Frequency
- **Bar Plot**:
  - Customers with higher purchase frequencies also exhibit higher spending, especially in Group B.

#### Post-Hoc Analysis Visualization
- **Tukey’s HSD Plot**:
  - Shows significant differences between subgroups, particularly in spending behaviors of `B_Long` compared to other categories.

---

## Technical Details

### Libraries Used
- **Python Libraries**:
  - pandas, matplotlib, seaborn for data manipulation and visualization
  - scipy.stats for hypothesis testing
  - statsmodels for post-hoc analysis

### Steps Performed

1. **Data Preprocessing**
   - Filled missing values in `CREDIT_LIMIT` and `MINIMUM_PAYMENTS` with median values.
   - Created new features:
     - `Total Spending`: Aggregation of purchases and cash advances.
     - `Group_Tenure`: Combination of experimental group and tenure.

2. **Exploratory Data Analysis**
   - Analyzed spending behaviors using summary statistics.
   - Created histograms, box plots, and bar plots to visualize differences.

3. **Statistical Testing**
   - Conducted a two-sample t-test to evaluate group differences in spending.
   - Used Tukey’s HSD for post-hoc analysis to explore subgroup differences.

4. **Insights and Reporting**
   - Segmented spending behaviors by tenure and purchase frequency.
   - Documented significant findings and visualizations for interpretation.

---

## Observations

1. **Spending Variance**: Group B customers exhibit slightly higher spending than Group A.
2. **Tenure Impact**: Long-tenured customers in Group B drive much of the observed differences in spending.
3. **Frequency Correlation**: Higher purchase frequencies are associated with increased spending, especially in Group B.

---

## Files Included
1. **Code**: Python scripts for analysis and visualization.
2. **Visualizations**: Saved as `.png` files for easy access.
3. **README.md**: Overview and detailed documentation for the project.

---

## Next Steps
- Expand analysis to include customer demographics (if available).
- Integrate machine learning to predict customer spending based on group assignment and tenure.
- Automate the pipeline for repeated analysis on updated datasets.

---

## Contact
For any queries or collaboration opportunities:
- **Email**: mpriyadharsini6599@gmail.com
- **LinkedIn**: [Priyadharsini Manivannan](https://www.linkedin.com/in/priyadharsini-manivannan/)
- **GitHub**: [Priyadharsini0605](https://github.com/Priyadharsini0605)

