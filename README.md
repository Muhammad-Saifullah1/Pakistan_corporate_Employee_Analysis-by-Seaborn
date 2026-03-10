# 📊 Pakistan Corporate Employee Analysis — Seaborn Visualization Suite

> A comprehensive exploratory data analysis (EDA) of Pakistan's corporate workforce using **20 Seaborn visualizations** to uncover patterns in salary, demographics, performance, and employee satisfaction.

---

## 📁 Dataset Overview

The dataset contains employee-level records from corporate organizations across major Pakistani cities. Key features include:

| Feature | Description |
|---|---|
| `Name` | Employee identifier |
| `Age` | Employee age |
| `Gender` | Male / Female |
| `City` | Karachi, Islamabad, Lahore, Quetta, etc. |
| `Department` | Engineering, Sales, HR, Finance, etc. |
| `Salary` | Monthly salary (PKR) |
| `Experience` | Years of professional experience |
| `Rating` | Performance rating score |
| `Projects_Completed` | Total projects delivered |
| `Satisfaction_Score` | Employee satisfaction (1–10) |
| `Education` | Matric / Intermediate / Bachelors / Masters |
| `Overtime_Hours` | Monthly overtime hours |
| `Bonus` | Annual bonus amount |
| `Leaves_Taken` | Leaves taken in a year |
| `Performance` | Performance tier (Average / Good / Excellent) |

---

## 📈 Visualization Guide

Each graph below was created with a specific analytical purpose to extract meaningful business insights.

---

### Graph 1 — Salary Distribution by Gender (Histplot)
**File:** `01_histplot.png`

**Purpose:** Understand how salary is distributed across the workforce, and whether a gender-based salary gap exists.

**Insight:** Reveals the shape of the salary distribution (normal, skewed, bimodal) and highlights whether male and female employees are concentrated at different salary bands.

---

### Graph 2 — Age Distribution by Gender (KDE Plot)
**File:** `02_kdeplot.png`

**Purpose:** Visualize the density of age groups for each gender using a smooth, continuous curve.

**Insight:** Identifies the dominant age brackets in the organization and shows if there is an age-based gender imbalance — for example, whether the female workforce is relatively younger than male counterparts.

---

### Graph 3 — City-wise Employee Count by Gender (Countplot)
**File:** `03_countplot.png`

**Purpose:** Compare the number of male and female employees across different cities.

**Insight:** Pinpoints geographic workforce distribution and highlights cities where gender diversity is strong or lacking — useful for regional HR planning.

---

### Graph 4 — Average Salary by Department & Gender (Barplot)
**File:** `04_barplot.png`

**Purpose:** Quantify and compare the mean salary across departments, broken down by gender.

**Insight:** Directly exposes departmental pay disparities and potential gender pay gaps within specific teams (e.g., Engineering vs. HR vs. Sales).

---

### Graph 5 — Salary Distribution by Department (Boxplot)
**File:** `05_boxplot.png`

**Purpose:** Show the full salary spread (median, quartiles, outliers) per department and gender.

**Insight:** Goes beyond averages — reveals salary inequality, outlier earners, and how compressed or spread out pay is within each department. Useful for equity analysis.

---

### Graph 6 — Salary Distribution by City (Violin Plot)
**File:** `06_violinplot.png`

**Purpose:** Display the full salary density distribution for male vs. female employees in each city using a split violin.

**Insight:** Combines the benefits of a boxplot and KDE — showing not just median/spread, but where salaries cluster most densely, per city and per gender.

---

### Graph 7 — Salary vs Experience (Scatterplot)
**File:** `07_scatterplot.png`

**Purpose:** Explore the relationship between years of experience and salary, colored by department and sized by rating.

**Insight:** Confirms (or challenges) whether experience translates to higher pay. Also reveals if certain departments reward experience more than others, and whether high-rated employees earn proportionally more.

---

### Graph 8 — Average Salary by Age (Lineplot)
**File:** `08_lineplot.png`

**Purpose:** Track how average salary trends with increasing age across the workforce.

**Insight:** Shows career earnings progression — whether salaries peak at a certain age, plateau early, or grow consistently. Useful for retention and compensation strategy.

---

### Graph 9 — Correlation Heatmap
**File:** `09_heatmap.png`

**Purpose:** Visualize linear correlations between all numeric variables in a single matrix.

**Insight:** Quickly identifies which variables are strongly related (e.g., Experience & Salary), which are independent, and flags potential multicollinearity — critical before building any predictive model.

---

### Graph 10 — Pairplot Analysis
**File:** `10_pairplot.png`

**Purpose:** Plot pairwise relationships between Age, Salary, Experience, and Rating — all segmented by gender.

**Insight:** Provides a holistic, multi-variable view in one chart. Diagonal KDE plots show individual distributions; scatter plots reveal cross-variable trends and gender-based clustering.

---

### Graph 11 — Rating by Department & Performance (Stripplot)
**File:** `11_stripplot.png`

**Purpose:** Show individual employee rating scores across departments, grouped by performance tier.

**Insight:** Reveals rating distributions at the individual level — avoiding aggregation bias. Shows whether high-performing employees consistently receive better ratings across all departments.

---

### Graph 12 — Satisfaction Score by City (Swarmplot)
**File:** `12_swarmplot.png`

**Purpose:** Display individual satisfaction scores city-by-city, separated by gender, without overlapping data points.

**Insight:** Highlights which cities have the most satisfied (or dissatisfied) employees and reveals gender-based satisfaction gaps at a granular level. Useful for location-specific HR interventions.

---

### Graph 13 — Average Rating by Department (Pointplot)
**File:** `13_pointplot.png`

**Purpose:** Compare mean ratings across departments for male and female employees, with confidence intervals.

**Insight:** The confidence intervals reveal statistical reliability — wide intervals mean high variability; narrow intervals suggest consistency. Useful for performance benchmarking by department and gender.

---

### Graph 14 — Salary by City, Gender & Performance (Catplot)
**File:** `14_catplot.png`

**Purpose:** Examine salary distributions across cities and genders, faceted by performance tier.

**Insight:** A multi-dimensional view: shows how being in a particular city, having a particular gender, *and* a particular performance level all interact to determine salary. Ideal for identifying compensation fairness issues.

---

### Graph 15 — Salary vs Experience (Jointplot — Hex Bin)
**File:** `15_jointplot_hex.png`

**Purpose:** Map the density of salary-experience combinations using hexagonal binning.

**Insight:** Hex bins reveal where most employees cluster in the experience-salary space — showing if the majority are low-experience/low-salary or if there is a broad spread. Marginal histograms provide individual variable context.

---

### Graph 16 — Age vs Salary (Jointplot — KDE)
**File:** `16_jointplot_kde.png`

**Purpose:** Show the joint density of age and salary using a 2D KDE contour, with marginal distributions.

**Insight:** Identifies the most common age-salary combinations and shows the concentration of the workforce. Useful for workforce planning and compensation benchmarking.

---

### Graph 17 — Experience vs Salary (Jointplot — Regression)
**File:** `17_jointplot_reg.png`

**Purpose:** Fit a regression line onto the experience vs salary scatter, with marginal distributions.

**Insight:** Quantifies the direction and strength of the experience-salary relationship. A steep slope signals strong experience premiums; a flat slope suggests experience is not the dominant salary driver.

---

### Graph 18 — Projects Completed vs Salary (Regplot)
**File:** `18_regplot.png`

**Purpose:** Examine whether completing more projects is associated with higher salaries.

**Insight:** Tests a core performance-pay assumption. If the regression line is flat, it suggests productivity (measured by projects) is not adequately rewarded — a potential retention risk.

---

### Graph 19 — Experience vs Salary by Gender (LMplot)
**File:** `19_lmplot.png`

**Purpose:** Plot separate regression lines for male and female employees to compare experience-salary trajectories.

**Insight:** Directly visualizes the gender pay gap as a function of experience — whether women earn less than men at the same experience level, and whether the gap widens over time.

---

### Graph 20 — Department Distribution (Pie Chart)
**File:** `20_piechart.png`

**Purpose:** Show the proportional headcount breakdown across all departments.

**Insight:** Immediately communicates organizational structure — which departments are largest and where workforce resources are concentrated. Useful for capacity planning and budgeting.

---

## 🛠️ Tech Stack

```
Python 3.x
├── pandas          — Data loading & manipulation
├── numpy           — Numerical operations
├── matplotlib      — Base plotting engine
└── seaborn         — Statistical visualization layer
```

---

## 🚀 How to Run

```bash
# 1. Clone the repository
git clone https://github.com/your-username/pakistan-employee-analysis.git
cd pakistan-employee-analysis

# 2. Install dependencies
pip install pandas numpy matplotlib seaborn

# 3. Run the analysis
python analysis.py
```

All 20 graphs will be saved as `.png` files in the working directory.

---

## 📌 Key Findings Summary

- **Salary & Experience** show a positive correlation, but the relationship varies significantly by department.
- **Gender pay gaps** are visible in certain departments — most notably in Engineering and Sales.
- **City-wise analysis** reveals that Karachi and Islamabad have higher average salaries compared to other cities.
- **Performance ratings** do not always align with salary levels, suggesting non-merit factors influence compensation.
- **Employee satisfaction** varies significantly by city, with gender-based differences present in most locations.

---

## 📄 License

This project is intended for educational and analytical purposes.

---

*Analysis performed on Pakistan Corporate Employee Dataset | Visualizations: Seaborn + Matplotlib*