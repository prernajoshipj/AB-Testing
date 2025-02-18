# 📊 A/B Testing for Mobile Game Retention

## 🏆 **Project Overview**
This project evaluates the impact of a newly introduced feature in a mobile game on **player retention**. The game company conducted an **A/B test** where:
- **Control Group (`gate_30`)**: Played the game without the new feature.
- **Test Group (`gate_40`)**: Played the game with the new feature enabled.

The goal is to determine whether the **new feature improves player retention** and affects **player engagement**.

---

## 📂 **Dataset**
The dataset used is from **Kaggle's "Mobile Games A/B Testing" dataset**, originally collected from the game *Cookie Cats*.

### **📌 Key Columns:**
- `userid`: Unique identifier for each player.
- `version`: Indicates the A/B test group (**'gate_30'** = Control, **'gate_40'** = Test).
- `sum_gamerounds`: Total number of game rounds played during the first week.
- `retention_1`: Whether the player returned the next day (**1 = Yes, 0 = No**).
- `retention_7`: Whether the player returned after 7 days (**1 = Yes, 0 = No**).

---

## 🎯 **Project Objectives**
✅ **1. Data Exploration & Cleaning**
- Inspect missing values, check dataset distribution, and perform necessary preprocessing.

✅ **2. Retention Analysis**
- Calculate and visualize **Day 1 & Day 7 retention rates** for both groups.
- Use **bar charts** to compare retention trends.

✅ **3. Statistical Testing**
- Perform a **Chi-Square Test** to determine if retention differences are statistically significant.
- Conduct a **t-Test** to analyze differences in game rounds played.

✅ **4. Player Engagement Analysis**
- Analyze whether the new feature affects the **number of game rounds played**.
- Use **histograms & log-scale visualization** to account for data skewness.

✅ **5. Predictive Modeling**
- Train a **Logistic Regression Model** to predict **Day 7 retention**.
- Evaluate model performance using **classification reports and heatmaps**.

✅ **6. Business Recommendations**
- Decide whether the feature should be rolled out based on statistical & predictive results.

---

## 📊 **Key Findings & Results**
- **Day 1 Retention** → ❌ **No significant difference** between the two groups.
- **Day 7 Retention** → ✅ **Significant improvement** in the test group.
- **Game Rounds Played** → ❌ **No significant difference** → Feature does not impact short-term engagement.
- **Survival Analysis** → ✅ **Players in the test group lasted longer** before dropping off.

### 🔬 **Statistical Test Results:**
| Test | Statistic | p-value | Interpretation |
|------|------------|--------|----------------|
| Chi-Square (Day 1 Retention) | 3.159 | 0.0755 | ❌ No significant difference |
| Chi-Square (Day 7 Retention) | 9.959 | 0.0016 | ✅ Significant improvement |
| t-Test (Game Rounds) | 0.891 | 0.3729 | ❌ No significant difference |

---

## ✅ **Final Recommendations**
🚀 **Keep the feature!** But optimize early engagement.
- **Long-term retention improves**, so rolling out the feature is beneficial.
- **Early engagement should be improved** → Add better **onboarding tutorials & rewards** to boost **Day 1 retention**.
- **Further A/B tests** → Test different onboarding experiences and engagement features.

---

## ⚡ **Installation & Usage**
### 🛠 **Requirements**
- Python 3.7+
- Jupyter Notebook
- Libraries: `pandas`, `matplotlib`, `seaborn`, `scipy`, `sklearn`, `tabulate`

### 🚀 **Run the Notebook**
```bash
# Clone the repository
git clone https://github.com/YOUR_GITHUB_USERNAME/AB_Testing_Game_Retention.git
cd AB_Testing_Game_Retention

# Open Jupyter Notebook
jupyter notebook abtest.ipynb
```

---

## 📎 **Project Structure**
```
📁 AB_Testing_Game_Retention/
│-- 📄 abtest.ipynb    # Jupyter Notebook with analysis & results
│-- 📄 cookie_cats.csv # Dataset 
```

---

## 👨‍💻 **Author**
Developed by **Prerna Joshi**
- 🔗 LinkedIn: www.linkedin.com/in/joshi-prerna
- 📧 Email: pxj7280@mavs.uta.edu

📌 **Feel free to contribute, report issues, or suggest improvements!** 🚀

