# 🏠 Airbnb NYC Listings Analysis

An exploratory data analysis of the New York City Airbnb Open Data dataset, examining pricing dynamics, host behavior, and guest review patterns across the city's short-term rental market.

## 📖 Problem Statement

Airbnb has reshaped the short-term lodging industry through a commission-based, host-guest marketplace model. This project analyzes the NYC Airbnb dataset to understand what drives listing availability, pricing, and guest satisfaction across New York's boroughs.

## ❓ Research Questions

1. What are the different property types in the dataset?
2. Which neighborhood group has the highest number of listings?
3. Which neighborhood groups have the highest average listing prices?
4. Is there a relationship between construction year and price?
5. Who are the top 10 hosts by calculated listing count?
6. Are hosts with verified identities more likely to receive positive reviews?
7. Is there a correlation between listing price and service fee?
8. How does average review rate vary by neighborhood group and room type?
9. Do hosts with more listings maintain higher year-round availability?

## 🧹 Data Wrangling

- Removed **541 duplicate records**
- Dropped columns with insufficient data (`house_rules`, `license`)
- Cleaned currency formatting (`$`, commas) from `price` and `service fee`
- Corrected data types across price, ID, host ID, review date, and construction year fields
- Fixed a misspelling in the `neighbourhood group` column (`brookln` → `Brooklyn`)
- Addressed outliers in the `availability 365` column

## 🔍 Key Findings

- **Entire home/apt** is the dominant property type (44,369 listings), followed by Private room (37,684)
- **Brooklyn** and **Manhattan** lead in listing volume (34,794 and 34,741 respectively)
- Average listing price shows a **downward trend** relative to construction year
- **Sonder (NYC)** tops the list of highest-volume hosts
- Host verification showed only a marginal effect on review rate (3.28 vs. 3.27)
- **Strong positive correlation (r = 0.99)** between listing price and service fee
- Hotel rooms had the highest review ratings across Brooklyn, Manhattan, and Queens
- Weak correlation (r = 0.135) between host listing count and year-round availability

## 🛠️ Tech Stack

`Python` · `Pandas` · `NumPy` · `Matplotlib` · `Seaborn` · `Plotly Express`

## ▶️ How to Run

```bash
pip install pandas numpy matplotlib seaborn plotly
jupyter notebook Adepu_Nalin_Kumar_Source_Code.ipynb
```

## ✅ Conclusion

This analysis surfaces actionable insights into NYC's short-term rental market — from pricing dynamics to host and review behavior — with potential extensions into sentiment analysis on guest reviews and predictive modeling for demand and pricing forecasts.

---
**Author:** [Nalin Kumar](https://github.com/nalinkumar2710) | Part of the AICTE–VOIS Conversational Data Analysis Virtual Internship (Sep–Oct 2025)
