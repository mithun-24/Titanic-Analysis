# Titanic Survival Analysis

Exploratory data analysis (EDA) of the Titanic passenger dataset to find out which factors influenced survival.

## Objective
Understand who survived the Titanic disaster and why, using data cleaning and visualization.

## Dataset
Titanic dataset loaded from the Seaborn library: 891 passengers and 15 features (age, sex, class, fare, etc.).

## Tools Used
Python, Pandas, NumPy, Matplotlib, Seaborn, Google Colab

## Data Cleaning
- Dropped the `deck` column (77% of values missing)
- Filled 177 missing `age` values with the median (robust to outliers)
- Dropped 2 rows with missing `embarked` values
- Final dataset: 889 rows, 14 columns

## Key Findings
1. **Overall:** Only about 38% of passengers survived.
2. **Sex:** Women survived at roughly 74% compared with about 19% for men, which is consistent with the "women and children first" policy.
3. **Class:** Survival dropped sharply with ticket class: roughly 63% in first class, 47% in second and 24% in third.
4. **Class + Sex:** Women in first and second class survived at over 90%, while third-class women survived at about 50%. Men in second and third class had the lowest survival (under 20%), so class mattered even within each gender.
5. **Age:** Young children had a noticeably higher survival rate, while most non-survivors were adults aged roughly 20-40.
6. **Fare:** The average fare (32) is much higher than the median (14), meaning a few very expensive first-class tickets skew the data.

## Conclusion
Survival was strongly linked to sex and passenger class, with age playing a smaller role. Women and first-class passengers had the best chances, and third-class men had the worst.

## How to Run
Open `Titanic_Analysis.ipynb` in Google Colab and run all cells.

## Next Steps
Build a machine learning model to predict survival (coming in a later project).
