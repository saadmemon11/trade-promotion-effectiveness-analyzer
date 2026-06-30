# 🚀 Trade Promotion Effectiveness Analyzer
### Python | Promotion Lift & ROI Analysis | FMCG Beverages & Snacks | India | FY 2023

---

## 📌 Project Overview

This project answers one of the most valuable questions in FMCG retail analytics: **are trade promotions actually driving incremental sales, or are customers simply buying what they would have bought anyway at a lower price?**

Using Python, this analysis measures **promotional lift** (extra volume generated above baseline), tests its **statistical significance**, and calculates **ROI** across promotion types, product categories, channels, regions, and individual SKUs — to determine which promotional strategies are genuinely profitable and which ones lose money despite driving volume.

---

## 🎯 Business Context

> A category manager running trade promotions for a brand would ask:
> - Do promotions cause a real, statistically significant increase in sales?
> - Which promotion type — discount, BOGO, display — delivers the best ROI?
> - Does discount depth keep increasing sales proportionally, or are there diminishing returns?
> - Which channels and regions respond best to which promotion type?
> - Which SKUs and categories should get more (or less) promotional investment?

This is the type of analysis that determines how millions of rupees in trade marketing budget get allocated each year.

---

## 📦 Dataset Details

| Attribute | Details |
|---|---|
| Total Rows | 6,656 |
| Time Period | Jan 2023 – Dec 2023 (52 weeks) |
| SKUs | 8 products across Carbonated Drinks, Energy Drinks, Juices, Water, Sports Drinks, Tea, Snacks, Confectionery |
| Regions | North India, South India, East India, West India |
| Channels | Modern Trade, Quick Commerce, E-Commerce, Kirana |
| Promotion Types | No Promotion, Light Discount (10%), Medium Discount (20%), Deep Discount (30%), BOGO, Display + Discount |
| Key Columns | Baseline Units, Actual Units Sold, Selling Price, Revenue, Promo Cost, Incremental Units, Incremental Revenue |

Dataset is synthetically generated with built-in realistic promotional response curves (including diminishing returns at higher discount depths) for portfolio purposes.

---

## 🔬 Analysis Workflow

| Step | What It Does |
|---|---|
| Data Cleaning | Duplicate checks, validation of incremental metrics, negative value checks |
| Executive KPI Summary | Total revenue, promo spend, incremental revenue, overall ROI |
| Promo vs Non-Promo Comparison | Baseline check — do promo weeks outsell regular weeks? |
| Statistical Significance Test | Independent t-test confirming the lift is real, not random variation |
| ROI by Promotion Type | Which promo types are profitable vs which lose money |
| Category & SKU Breakdown | Incremental revenue and ROI ranked by product |
| Channel × Promotion Heatmap | Cross-tab showing where each promo type performs best |
| Discount Depth Regression | Linear regression testing for diminishing returns on deeper discounts |
| Monthly Trend Analysis | Promotional spend vs incremental revenue across the year |
| Regional Effectiveness | ROI and incremental revenue by region |

---

## 📊 Key Findings

- **Promotions cause a statistically significant lift** in unit sales (t-test, p < 0.05) — confirming the effect is real, not random variation
- **Display + Discount delivers the strongest ROI (+126%)**, while **BOGO promotions return -87% ROI** despite generating the highest raw unit volume — proving that volume lift and profitability are not the same thing
- **Discount depth shows clear diminishing returns** (R² = 0.72) — each additional percentage point of discount generates progressively less incremental volume
- **Modern Trade and Kirana channels respond strongest to BOGO and Display+Discount promotions**, based on the channel × promotion heatmap
- **Light and Medium discounts are the only consistently profitable promotion types** when promo cost is factored against incremental revenue
- **Regional ROI varies meaningfully**, suggesting promotional budgets should be region-specific rather than applied uniformly nationwide

---

## 🛠️ Tools & Libraries

- **Python 3.12**
- **Pandas** — data manipulation and aggregation
- **NumPy** — numerical operations
- **Matplotlib & Seaborn** — custom dark-themed data visualization (9 charts)
- **SciPy** — independent t-test for statistical significance
- **Scikit-learn** — linear regression for discount-lift relationship

---

## 📈 Visualizations

1. KPI Dashboard — Total Revenue, Promo Spend, Incremental Revenue, Overall ROI
2. Promo vs Regular Week Comparison (Units & Revenue)
3. ROI by Promotion Type (horizontal bar)
4. Incremental Revenue by Category
5. Channel × Promotion Type Heatmap
6. Discount Depth vs Incremental Lift (scatter + regression line)
7. Monthly Promotional Spend vs Incremental Revenue
8. SKU Promotional ROI Ranking (bubble chart)
9. Regional Promotional Effectiveness (ROI & Revenue)

All charts use a custom dark navy theme with cyan, gold, green, and red accents to match the rest of the portfolio.

---

## 📁 Files in This Repository

```
├── Promotion_Lift_Analysis.ipynb     # Full Jupyter notebook with analysis
├── promotion_sales_data.csv          # Dataset (6,656 rows)
├── Screenshots/
│   ├── KPI_Dashboard.png
│   ├── Promo_vs_Non-Promo.png
│   ├── ROI_by_Promotion_Type.png
│   ├── Heatmap_Channel_Promo.png
│   ├── Regression_Analysis.png
│   └── SKU_Bubble_Performance.png
└── README.md
```

---

## 🚀 How to Use

1. Clone or download this repository
2. Install dependencies: `pip install pandas numpy matplotlib seaborn scipy scikit-learn`
3. Open `Promotion_Lift_Analysis.ipynb` in Jupyter Notebook or VS Code
4. Ensure `promotion_sales_data.csv` is in the same folder
5. Run all cells to reproduce the full analysis and charts

---

## 👤 About

Built by **Saad** — CS Engineering Student at Parul University transitioning into Data Analytics.

This project completes a **4-part FMCG and retail analytics portfolio** spanning Power BI, Excel, MySQL, and Python — simulating real-world data work across the full analytics toolchain used in the consumer goods and retail analytics space.

🔗 [LinkedIn](https://linkedin.com/in/saad-memon-49aa75350) | 📧 saadmemon1104@gmail.com | 🐙 [GitHub](https://github.com/saadmemon11)
