# Week 7: Data Transformation & Feature Engineering

In this **Week 7 project**, I focused on transforming my cleaned supply chain dataset into a richer, more insightful version using **Pandas**. This week was about handling missing values, converting data types, cleaning text, and creating new columns to reveal patterns hidden in the raw data.  

Feature engineering helped me generate new information that directly answered business questions.

![Project Introduction](https://github.com/R887645/TDI-Python-Learning-Week-7-Project-/blob/main/Intro.png?raw=true)

---

# Key Skills Practiced

- Detecting and handling missing values with `.isnull()`, `.fillna()`, and `.dropna()`
- Converting data types using `pd.to_datetime()`, `pd.to_numeric()`, and `.astype()`
- Creating new columns from existing ones *(delivery duration, profit margin, efficiency score, delay status)*
- Cleaning text data with `.str.strip()`, `.str.lower()`, and `.str.replace()`
- Categorizing continuous data into bins for easier grouping and analysis

---

# What I Implemented

## 1. Handling Missing Values

I identified missing values across columns, counted them, and applied strategies:

- Filled numeric columns with their **mean values**
- Filled categorical columns with their **most frequent value (mode)**
- Dropped rows where **too many values were missing**

![Handling Missing Values](https://github.com/R887645/TDI-Python-Learning-Week-7-Project-/blob/main/Task1.png?raw=true)

---

## 2. Data Type Conversion

I converted text columns into **numeric and datetime formats** to enable calculations.

This included converting:

- `order_date`
- `delivery_date`

into proper **datetime objects**, and ensuring **cost** and **quantity** were numeric values.

---

## 3. Creating New Columns

I engineered new features to answer business questions:

- **Delivery duration (`delivery_days`)** from order and delivery dates
- **Order profit (`order_profit`)** using cost, quantity, and margin
- **Efficiency score (`efficiency_score`)** comparing lead time vs actual delivery days
- **Delay status** *(On Time or Delayed)* based on expected vs actual delivery

![Feature Engineering](https://github.com/R887645/TDI-Python-Learning-Week-7-Project-/blob/main/Task2.png?raw=true)

---

## 4. String Cleaning

I standardized **supplier names** and **product categories** by:

- Removing extra spaces using `.str.strip()`
- Standardizing case using `.str.lower()`
- Replacing inconsistent text formatting

This ensured consistency across the dataset.

---

## 5. Categorizing Continuous Data

I grouped continuous values into categories for easier analysis:

- **Cost ranges:** Low, Medium, High
- **Delivery speed:** Fast, Moderate, Slow

This made grouping and comparison easier during analysis.

---

# Reflection

This project showed me how **feature engineering transforms raw data into actionable insights**. By handling missing values, converting data types, and creating new columns, I built a cleaner and richer dataset.  

Text cleaning and categorization also made grouping and analysis more intuitive.

One challenge I faced was deciding the **best strategy for handling missing values — whether to fill or drop them**. I learned that the choice depends on the **proportion of missing data and the importance of the column**.

Overall, **Week 7 helped me move from data preparation into true transformation**, setting the stage for deeper analysis with **grouping and summary statistics in Week 8**.

---

# View the Full Project

🔗 **View my Week 7 full project here:**  
https://github.com/R887645/TDI-Python-Learning-Week-7-Project-
