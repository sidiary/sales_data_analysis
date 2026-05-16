# sales_data_analysis
#  Pharma Sales Data Analysis
### AI Academia — Python with Data Science Internship | [Sidra Ahmed] | May 2026

---

##  About

End-to-end analysis of a pharmaceutical sales dataset spanning **2014–2019**, covering over **10,000 transactions** across 8 drug categories, 5 regions, and 4 sales channels.

The project includes data cleaning, exploratory data analysis, statistical hypothesis testing, and two machine learning models — linear regression for sales forecasting and logistic regression for high/low sale classification.

---

## Tools Used

| Tool | Purpose |
|---|---|
| Python 3.13 | Core programming language |
| Pandas | Data loading, cleaning, manipulation |
| NumPy | Statistical computations |
| Matplotlib | Line, bar, and pie charts |
| Seaborn | Heatmap and boxplot visualisations |
| Scikit-learn | Linear regression & logistic classification |
| SciPy | Hypothesis testing (t-test) |

---

##  Dataset

- **Source:** Pharmaceutical sales dataset (2014–2019)
- **Rows:** ~10,000+ transactions after cleaning
- **Columns:** 9 (Date, Product, Category, Region, Channel, Quantity, Unit Price, Discount, Sales)
- **Drug Categories:** 8 ATC classification codes including analgesics, anti-inflammatories, anxiolytics, antihistamines
- **Raw data issues fixed:** Mixed date formats, duplicate rows, negative sales values, outliers, missing values, inconsistent capitalisation

---

##  Project Structure

```
sales-data-analysis/
│
├── sales_analysis_final.ipynb   # Main analysis notebook
├── pharma_sales_raw (1).csv         # Raw dataset (messy)
├── README.md                    # This file
│
├── monthly_trend_final.png      # Annotated monthly sales trend
├── category_sales.png           # Sales by drug category
├── region_sales.png             # Regional sales pie chart
├── heatmap.png                  # Correlation heatmap
├── boxplot.png                  # Sales distribution by category
├── seasonal.png                 # Average sales by month
├── distribution.png             # Sales distribution histogram
├── regression.png               # Actual vs predicted sales
└── confusion_matrix.png         # Classification model results
```

---

##  Notebook Sections

| Section | Content |
|---|---|
| 1 — Data Loading | Load CSV, inspect shape, columns, and data types |
| 2 — Data Cleaning | Fix dates, remove duplicates, handle nulls and outliers |
| 3 — NumPy Statistics | Mean, median, std dev, best/worst months |
| 4 — Matplotlib Charts | Line, bar, and pie charts with annotations |
| 5 — Seaborn Charts | Correlation heatmap and category boxplot |
| 6 — EDA Report | Top/bottom products, seasonal trends, key findings |
| 7 — Hypothesis Testing | Skewness, percentiles, t-test between categories |
| 8 — Linear Regression | Monthly sales prediction with MAE and R² |
| 9 — Classification | High/Low sale prediction with confusion matrix |

---

##  Key Findings

**Finding 1:** The top drug category (analgesics/anti-inflammatories) dominates total revenue across all regions.
- **Meaning:** Over-reliance on a narrow set of drug categories creates supply chain and revenue risk.
- **Action:** Diversify the portfolio by growing under-represented categories like N05B and N05C.

**Finding 2:** Winter months (November–February) generate 25–35% more sales than the annual monthly average.
- **Meaning:** Cold-weather conditions significantly drive demand for analgesics and anti-inflammatory drugs.
- **Action:** Begin procurement planning in September to ensure adequate stock before the November peak.

**Finding 3:** The top 3 individual products account for a disproportionate share of total revenue vs the bottom 3.
- **Meaning:** A classic Pareto distribution — a small number of drugs drive the majority of business value.
- **Action:** Prioritise stock availability and competitive pricing for these top products year-round.

**Finding 4:** Discount rate has a negative correlation with Sales value per transaction.
- **Meaning:** Blanket discounting reduces revenue per transaction without a proportional volume increase.
- **Action:** Reserve discounts for slow-moving SKUs only — never discount top-selling products.

**Finding 5:** Regional revenue is balanced across all five regions with no area exceeding 25% of total sales.
- **Meaning:** The distribution network has no critical geographic dependency or single point of failure.
- **Action:** Focus incremental marketing investment on the lowest-performing region to unlock new growth.

---

##  Recommendations

1. **Seasonal inventory forecasting** — Place procurement orders 6–8 weeks before the November peak to prevent stockouts of high-demand analgesics during winter months.

2. **Restructure discount strategy** — Since discounting negatively correlates with sales revenue, apply promotional pricing only to categories with below-average sales velocity, not to top-performing products.

---

##  How to Run

```bash
# Install dependencies
pip install pandas numpy matplotlib seaborn scikit-learn scipy

# Open the notebook
jupyter notebook sales_analysis_final.ipynb
```

Or open `sales_analysis_final.ipynb` directly in **VS Code** with the Jupyter extension installed,  
select the correct Python kernel, and click **Run All**.

---

##  Author

**Sidra Ahmed**  
AI Academia — Python with Data Science Internship, 2026  
