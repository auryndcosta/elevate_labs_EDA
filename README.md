# Task 5: Exploratory Data Analysis (EDA)

## Objective
The primary goal of this task was to extract insights from the dataset using visual and statistical exploratory data analysis techniques.I aimed to understand the distribution of key features, uncover relationships between variables, and summarize trends in the data.

---

## Tools & Libraries Used
- **Python**
- **Pandas**: For data manipulation and summarization.
- **Matplotlib & Seaborn**: For data visualization.

---

## Files Included
- `eda_analysis.ipynb` - Jupyter Notebook containing all the code and visuals.
- `train.csv` - csv file containing titanic data.

---

## Key Techniques and Functions Used

### Statistical Summary & Inspection
- `df.info()`, `df.describe()` - To understand the structure and basic statistics of the dataset.
- `df['Survived'].value_counts()` - To evaluate class distribution.

### Visualizations Performed
- **Countplot** of Survived: To view the number of survivors vs non-survivors.
- **Pie Chart**: `df['Survived'].value_counts().plot(kind='pie')` to show survival distribution in percentage.
- **Histogram & Distplot**: To analyze the distribution of age.
  - `plt.hist(df['Age'])`
  - `sns.distplot(df['Age'])`
- **Boxplot**: `sns.boxplot(df['Age'])` to detect outliers and understand the spread of age.
- **Crosstab with Heatmap**:
  - `pd.crosstab(df['Pclass'], df['Survived'])` to explore class-wise survival rates.
  - `sns.heatmap(...)` to visualize it.
- **Pairplot**: `sns.pairplot(df)` to examine pairwise relationships between variables.

---

## Observations
Each visual was accompanied by interpretations, including:
- Survival distribution is imbalanced.
- Age is slightly right-skewed with visible outliers.
- Class appears to influence survival — higher classes had higher survival rates.
- No strong linear correlations, but some categorical variables impact survival.

---

## Summary of Findings
- **Survival Rate**: Majority did not survive; significant class-wise disparity.
- **Age Distribution**: Concentrated between 20-40 years, with outliers present.
- **Class-Survival Relationship**: Higher classes had better survival chances.
- **Visual Patterns**: Boxplots and heatmaps helped highlight group-wise differences and outliers.

---

## Deliverables
- Jupyter Notebook (.ipynb)
- PDF Report (.pdf)


