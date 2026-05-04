# 🏠 Nepal Housing Price Analysis
### WorldQuant University — Applied Data Science Lab
### Project 1: Housing in Mexico (adapted to Nepal)
### Lesson 1: Tabular and Tidy Data

---

## 📌 What This Lesson Is About
Learning how to organize housing data properly in Python
so it's ready for analysis.

---

## 🗂️ Tidy Data Rules
1. Each **row** = one house (called an observation)
2. Each **column** = one characteristic like price or area (called a feature)
3. Each **cell** = only one value

---

## 🧠 Key Concepts Learned

### Lists
- Store multiple values in one variable
- Problem: you can't tell what each number means
- Example: `[8500000, 120, 3]` — which is price? which is area?

### Dictionaries
- Solve the list problem by adding labels (keys) to each value
- Example: `{"price_npr": 8500000, "area_sqm": 120, "rooms": 3}`
- Much easier to understand and work with

### Row-wise vs Column-wise
- **Row-wise** (list of dicts): easy to work with one house at a time
- **Column-wise** (dict of lists): easy for calculations across all houses
- Each has tradeoffs depending on what you want to do

### For Loops
- Used to automate repetitive tasks
- Instead of calculating price per sqm for each house manually,
  we let the loop do it for all houses automatically

### zip()
- Lets you loop through two lists at the same time
- Used here to pair each price with its matching area

### Pandas DataFrame
- Best of both worlds — supports both row and column operations
- Much more powerful than plain lists or dictionaries

---

## 💡 My Key Insight
Column-wise organization makes aggregations like mean price easy,
but row-wise operations like adding price per sqm become harder.
Pandas solves both problems elegantly.

---

## 🛠️ Libraries Used
- `pandas`
