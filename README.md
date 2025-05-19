# 🍽️ Zomato Restaurants Data Analysis & Recommendation System

This project explores and analyzes the Zomato restaurant dataset with a focus on Indian restaurants. It includes comprehensive data cleaning, visualizations, and a custom-built restaurant recommendation system based on cuisine, city, rating, and cost.

---

## 📦 Dataset

- Source: [Zomato Restaurants Dataset on Kaggle](https://www.kaggle.com/datasets/shrutimehta/zomato-restaurants-data)
- File: `zomato.csv`
- Country Filter: India only (Country Code = 1)

---

## 🔧 Features Implemented

### 1. **Data Cleaning & Preparation**
- Normalized column names
- Filtered out non-Indian restaurants
- Removed rows with missing cuisine, rating, or votes

### 2. **Exploratory Data Analysis (EDA)**
- 📍 Top 10 Cities with Most Restaurants
- 💸 Distribution of Average Cost for Two
- ⭐ Distribution of Aggregate Ratings
- 🍜 Most Popular Cuisines

### 3. **Recommendation System**
- Content-based filtering using:
  - Cuisines
  - City
  - Average Cost
  - Aggregate Rating
- Cosine similarity (text + numeric features)
- Function: `recommend_restaurants(restaurant_name, top_n=5)`

---

## 🖼️ Visualizations
All plots are generated using `matplotlib` and `seaborn`:
- Bar plots for top cities and cuisines
- Histograms for cost and ratings

---

## 🧠 Example Usage

```python
# Recommend 5 restaurants similar to "Domino's Pizza"
recommend_restaurants("Domino's Pizza", top_n=5)


zomato_data_analysis/
├── zomato.csv
├── zomato_analysis.py       # Main code file
├── README.md                # This file


pip install pandas matplotlib seaborn scikit-learn
