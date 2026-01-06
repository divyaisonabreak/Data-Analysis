# Movie Rentals | Revenue & Content Performance (Power BI) — Sakila Dataset

This project is a Power BI dashboard built on the **Sakila** sample database (public movie rental dataset).  
The goal is to replicate a real-world reporting scenario: **summarize platform performance**, identify **revenue drivers**, and create a foundation for deeper content and customer analysis.

---

## Dashboard Pages

### Page 1: Overview (Executive Summary)
Designed to answer:
- How are rentals and revenue performing overall?
- What content is driving revenue (categories + titles)?
- How does performance change over time?

### Page 2: Content Performance
Designed to answer:
- Which titles are rented the most?
- How does revenue vary by **rating**?
- What changes when filtering by **rating** and **category**?

**Interactivity**
- Slicers: **Rating**, **Category**
- Cross-filtering enabled (clicking bars filters other visuals + table)

---

## Key Metrics (Overall)
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

## Measures (Definitions)
*(Names may vary depending on your PBIX, but definitions should match this logic.)*
- **Total Revenue** = Sum of payment amount  
- **Total Rentals** = Count of rentals (rows or distinct `rental_id`)  
- **Customers** = Distinct count of `customer_id`  
- **Revenue per Rental** = `Total Revenue / Total Rentals` (use `DIVIDE` to avoid divide-by-zero)

---

## Data & Modeling Notes
- Source: **Sakila** (public sample database)
- Data imported into Power BI and modeled with fact-style rental/payment reporting (often through a consolidated SQL view).
- Measures created in DAX (Revenue, Rentals, Customers, Revenue per Rental, etc.)

---

## Tools Used
- **SQL** (Sakila dataset)
- **Power BI** (data model, DAX measures, visuals)

---

---

## How to Run
1. Load the **Sakila** database into your SQL environment.
2. Open Power BI Desktop and connect to the database.
3. Import tables + create relationships (or use your consolidated SQL view).
4. Open the `.pbix` file and **Refresh**.

---

## Screenshots

### Page 1: Overview
<img width="1303" height="733" alt="image" src="https://github.com/user-attachments/assets/ec313a65-1ccd-47e2-bcf9-e41a50055ab7" />

### Page 2: Content Performance
<img width="1303" height="737" alt="image" src="https://github.com/user-attachments/assets/a49c3fba-ef42-463a-859c-36aa0f68ea4f" />

> Add your Page 2 screenshot to `/assets/page2_content_performance.png` and reference it below:
<img width="1302" height="735" alt="Page 2 - Content Performance" src="./assets/page2_content_performance.png" />
