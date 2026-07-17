# 📊 Cohort Retention Analysis — Olist E-Commerce

Customer retention analysis using a cohort-based approach to understand purchasing behaviour over time.

**Business Question:** How long do customers remain active after their first purchase — and what does this mean for the business?

---

## 📋 Project Overview

Olist is a Brazilian e-commerce marketplace selling durable goods (electronics, home appliances, furniture). Using transactional data from 100k+ orders, customers were grouped into monthly cohorts based on their first purchase date, and retention rates were tracked over time.

**Hypothesis going in:** Most customers make only one purchase — retention will be low due to the nature of the business model (durable goods marketplace).

---

## 📊 Key Findings

| Months after first purchase | Average Retention Rate |
|-----------------------------|------------------------|
| Month 1 | 0.5% |
| Month 2 | 0.3% |
| Month 3 | 0.3% |
| Month 6 | 0.3% |

**The hypothesis was confirmed.** Retention drops to near zero after the first purchase across all cohorts (2017–2018).

### Retention Heatmap
![Retention Heatmap](outputs/retention_heatmap.png)

---

## 💡 Business Conclusions

Low retention is **not a failure** — it reflects the business model. Customers buying electronics or furniture do not repurchase within months. However, this creates a structural dependency on new customer acquisition.

**Recommendations:**

| Priority | Action |
|----------|--------|
| 🔴 **High** | Expand into high-frequency categories (consumables, accessories) to drive repeat purchases |
| 🟡 **Medium** | Introduce a loyalty programme or next-purchase discount to incentivise return visits |
| 🟡 **Medium** | Offer value-added services (free delivery, installation, extended warranty) to increase purchase value |
| 🟢 **Lower** | Run personalised remarketing campaigns (email, product recommendations) to re-engage dormant customers |

---

## 🔧 How to Reproduce

1. Clone the repository:
   ```bash
   git clone https://github.com/leontiewaa/cohort-retention-analysis.git
   cd cohort-retention-analysis
   ```

2. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn jupyter
   ```

3. Add the Olist dataset to `data/raw/`:
   - Download from [Kaggle — Brazilian E-Commerce Dataset](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)
   - Place `olist_orders_dataset.csv` and `olist_customers_dataset.csv` in `data/raw/`

4. Open and run `notebooks/02_Cohort_Analysis.ipynb`

---

## 🛠️ Stack

| Tool | Purpose |
|------|---------|
| **Python (pandas, numpy)** | Data loading, cleaning, cohort calculations |
| **matplotlib, seaborn** | Retention heatmap visualisation |
| **Jupyter Notebook** | Development environment |

---

## 📂 Data Source

[Brazilian E-Commerce Public Dataset by Olist](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce) — real e-commerce data (100k+ orders), Kaggle.

---

## 📅 Status

✅ Completed — July 2026
