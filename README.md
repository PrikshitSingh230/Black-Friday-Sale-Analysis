# Black Friday Order Analysis 🛍️

---

### Project Overview

This notebook analyzes **500K+ rows**, covering **17K+ transactions** by **5,891 unique users**, **3,623 products**, and **18 product categories**.
The work focuses on cleaning the data, enriching key columns, and exploring orders by customer and product segments.

---

### Tools & Technologies

* **Jupyter Notebook (Python)**
* **pandas / numpy** for data processing
* **matplotlib / seaborn / plotly** for charts and visuals

---

### Data Source

Data obtained from **Kaggle** (Black Friday transactions export).

---

### Notebook Steps & Structure

1. **Preprocess & Clean**

   * Loaded raw CSV(s), fixed types, handled missing values and duplicates.

2. **Add simple derived columns**

   * `marital_gender` — combined marital status + gender.
   * `AgeBracket` — grouped ages into **teen / adult / senior**.

3. **Segmented analysis**

   * Single-column analysis: **Gender**, **AgeBracket**, **Marital Status**, **City Category**, **Stay_In_Current_City_Years**, **Occupation**, **Product Category**.
   * Pairwise analysis: combinations such as **Gender × AgeBracket**, **Gender × Occupation**, **AgeBracket × Product Category**, etc.

4. **Product & customer summaries**

   * Ranked top products by orders and by revenue.
   * Identified repeat buyers and high-value customers using order counts and total spend.

5. **Outputs**

   * Notebook with charts and tables; summary CSVs for top products and top customers.

---

### Analysis Highlights (what I checked)

* Gender: order counts, average purchase per user, share of total revenue by gender.
* AgeBracket: total orders and average order value per bracket.
* Marital & combined `marital_gender`: repeat purchase behavior and average spend by group.
* City category & stay-in-city years: order volumes and stability of buyers by locality.
* Occupation: order count and average spend per occupation group.
* Product category: which categories drive most orders and which have higher revenue per order.
* Pairwise checks: e.g., how gender + age bracket or occupation + age affect product preference.

---

### Business Insights (simple, formal, friendly)

* **Male customers are the larger buyer group.**
  Analysis shows men account for a higher share of total orders and overall spend compared with women.

* **Adults make the most purchases.**
  The `AgeBracket = adult` group records the highest order counts and contributes the largest share of revenue.

* **Married males show stronger value signals.**
  The `marital_gender` combination for married males has higher average order value and more repeat orders than many other groups.

* **City category and time-in-city matter.**
  One city category (noted in the notebook) has the highest order volume; customers who have lived longer in their current city show higher order frequency.

* **Certain occupations buy more and spend more.**
  A few occupation groups show above-average order counts and higher average order values (see occupation table in the notebook).

* **Product category concentration.**
  A small set of product categories account for a large share of orders; many SKUs form a long tail with low order counts.

* **Top customers identified by frequency and spend.**
  The notebook lists the highest-value users by total spend and by repeat orders (top buyers are shown in the summary table).

---

### Deliverables in the repo / notebook

* Cleaned notebook (.ipynb) : [JupyterNotebook](https://github.com/PrikshitSingh230/Black-Friday-Sale-Analysis/blob/main/BlackFriday%20Analysis.ipynb)
* CSV exports: [CSV](https://github.com/PrikshitSingh230/Black-Friday-Sale-Analysis/blob/main/BlackFriday.csv)


---

### Closing (short & clear)

This notebook turns raw Black Friday transactions into clear, factual insights about who buys most, which products and categories drive orders, and how locality and demographics affect buying. All results are in the notebook with supporting tables and charts.
