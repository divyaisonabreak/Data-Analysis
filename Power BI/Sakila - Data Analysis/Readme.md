# Movie Rentals | Revenue Overview (Power BI) — Sakila Dataset

This project is a Power BI dashboard built on the **Sakila** sample database (public movie rental dataset).  
The goal is to replicate a real-world reporting scenario: **summarize platform performance**, identify **revenue drivers**, and create a foundation for deeper content and customer analysis.

---

## Dashboard Preview (Page 1: Overview)
**Page 1** is an executive summary designed to answer:
- How are rentals and revenue performing overall?
- What content is driving revenue (categories + titles)?
- How does performance change over time?

---

## Key Metrics (Overview Page)
- **Total Rentals:** ~16K  
- **Total Revenue:** ~67.42K  
- **Revenue per Rental:** ~4.20  
- **Customers:** 599  

---

## Key Insights
### 1) Revenue is concentrated in a few categories
A small set of categories drives a large portion of total revenue:
- **Sports** leads overall, followed by **Sci-Fi** and **Animation**

### 2) Top titles consistently generate the most revenue
A handful of films repeatedly appear among the highest earners (e.g., *Telegraph Voyage*, *Wife Turn*, *Zorro Ark*).  
This supports practical actions like feature placement, bundling, or promotion testing.

### 3) Trend monitoring is clearer at Year-Month level
Using a Year-Month view reduces noise and makes incomplete periods easier to interpret.

---

## Data & Modeling Notes
- Source: **Sakila** (public sample database)
- Data imported into Power BI and modeled with fact-style rental/payment reporting through a consolidated view.
- Measures were created in DAX (Revenue, Rentals, Customers, Revenue per Rental, etc.)

---

## Tools Used
- SQL (Sakila dataset)
- Power BI (data model, DAX measures, visuals)

---

## Future Work
Planned additions in upcoming pages:
- **Content Performance Deep Dive** (rating/language/category mix, heatmaps, decomposition tree)
- **Customer Analytics** (repeat rentals, cohorts/retention, active vs inactive)
- **Geography** (revenue by country/city)
- **Pricing checks** (standard rental rate vs realized payment behavior)

---

## How to Run
1. Load Sakila database into your SQL environment.
2. Connect Power BI to the database.
3. Import tables + create relationships (or use a consolidated view).
4. Open the `.pbix` file and refresh.

---

## Screenshots
Add screenshots to `/assets/` and reference them here:
- `assets/page1-overview.png`

---

**Author:** <Your Name>  

