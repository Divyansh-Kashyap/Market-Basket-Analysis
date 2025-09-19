# Market-Basket-Analysis

## 📌 Overview

This project implements Market Basket Analysis (MBA), a data mining technique used by retailers to discover patterns and associations between items frequently purchased together.
By applying association rule learning, the project identifies strong rules such as:
👉 “If a customer buys bread, they are also likely to buy butter.”

The analysis provides insights for:

- Product bundling

- Cross-selling strategies

- Store layout optimization

- Personalized recommendations

## 📂 Project Structure
```
├── Market Basket Analysis.ipynb   # Jupyter Notebook with full implementation
├── README.md                      # Project documentation
└── dataset/                       # Transaction dataset

```
## 🔑 Key Features

- Exploratory Data Analysis (EDA):

-- Missing value analysis

-- Distribution of categorical features

-- Top 20 most purchased items

-- Visualization of item frequencies

- Data Cleaning & Preprocessing:

-- Handling null values

-- Formatting categorical data

-- Grouping transactions by Invoice

- Frequent Itemset Mining:

--- Implemented using Apriori Algorithm (via mlxtend)

-- Extracts frequent itemsets with support values

- Association Rule Learning:

-- Generates rules with metrics: Support, Confidence, Lift

-- Helps uncover hidden relationships between products

- Visualization:

-- Bar plots for top items

-- Heatmaps for co-occurrence

-- Support vs Confidence scatter plots

## 📊 Dataset

The dataset contains transactional records with columns like:

- InvoiceNo → Unique transaction ID

- Description → Product name

- Quantity → Number of items purchased

- InvoiceDate → Date of purchase

- UnitPrice → Price per unit

- CustomerID → Unique customer identifier

- Country → Country of customer

Each row represents one item purchased in a transaction.

## ⚙️ Tech Stack

- Programming Language: Python

Libraries:

- pandas, numpy → Data manipulation

- matplotlib, seaborn → Visualization

- mlxtend → Apriori algorithm & association rules

- itertools → Pairwise analysis (fallback)

## 🚀 How to Run

Clone the repository:
```
git clone https://github.com/your-username/market-basket-analysis.git
cd market-basket-analysis
```

Install dependencies:
```
pip install -r requirements.txt

```
Launch Jupyter Notebook:

jupyter notebook "Market Basket Analysis.ipynb"


Run all cells to generate EDA, itemsets, and association rules.

## 📈 Results

- Frequent itemsets identified (e.g., {Bread, Butter}, {Milk, Sugar})

- Strong association rules discovered with high confidence and lift

- Insights can be directly applied for:

- Product placement

- Promotional campaigns

- Personalized recommendations

## 🔮 Future Enhancements

- Deploy as a dashboard using Streamlit or Dash.

- Extend analysis with FP-Growth algorithm for scalability.

- Integrate with real-time transaction data for dynamic recommendations.
