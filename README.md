 🚢 Titanic Dataset - Exploratory Data Analysis (EDA)

📌 Task Objective

Perform exploratory data analysis (EDA) on the Titanic dataset to understand patterns, feature distributions, and relationships using statistical summaries and visualizations.

 🛠️ Tools Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn



 📁 Dataset Used

- `cleaned_titanic.csv` — This dataset was cleaned and preprocessed in Task 1, including:
  - Missing value treatment
  - Encoding categorical variables
  - Feature scaling
  - Outlier removal



 📊 Steps Performed

 1. Summary Statistics
- Used `.describe()` to view mean, median, std, min, max for each feature
- Found class imbalance: Only ~33% survived

 2. Histograms
- Visualized distribution of `Age`, `Fare`, `Pclass`, `SibSp`, and `Parch`
- Found most passengers were in 3rd class and paid lower fares
- Majority of passengers traveled alone

 3. Boxplots
- Detected outliers in `Age` and `Fare` visually
- Confirmed outlier removal done in preprocessing was effective

 4. Correlation Matrix
- Analyzed feature relationships
- Key findings:
  - `Sex_male` had a strong negative correlation with `Survived`
  - `Pclass` and `Fare` also correlated with survival
  - Other features had weak or no correlation

 5. Pairplot
- Explored interactions visually
- Observed survivors (orange dots) were mostly:
  - In higher classes
  - Female (`Sex_male = 0`)
  - Paid higher fares

 🔍 Key Insights

- Females and first-class passengers had better survival rates
- Fare and Pclass are important features
- About 33% of passengers survived, indicating data imbalance.
- Most passengers were in 3rd class; very few were in 1st class.
- Most had no siblings/spouses or parents/children onboard.
- Age and Fare were standardized. Most values are close to the mean, with few extremes.
- These insights will help guide visual exploration.
- Positive correlation seen between Fare and Survived.
- Negative correlation between Pclass and Survived — higher class passengers survived more.
- Strong negative correlation between Sex_male and Survived, confirming women had higher survival chances.
- Pairplot shows clear clusters for survivors, especially among higher-paying and younger passengers.
- Sex_male shows a strong negative correlation with survival (-0.51), indicating females had a higher chance of survival.
- Passengers in higher classes (Pclass=1) were more likely to survive.
- Fare is positively correlated — passengers who paid higher fares survived more, likely due to better cabins.
- Other features like SibSp, Parch, and Age show weak correlations.
- Most passengers were in 3rd class and traveled alone
- EDA highlighted imbalanced survival and feature relationships useful for ML



 📦 Files in this Repository

- `cleaned_titanic.csv` — Clean dataset
- `titanic_eda.ipynb` — Code for EDA
- `README.md` — This file


 ✅ Task Completed As Part of:
AI & ML Internship - Task 2


