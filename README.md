# NovaEra Retail – Business Intelligence Dashboard (Demo)

📊 **Overview**  
This project simulates a fictitious retail company called **NovaEra Retail S.A.**, using synthetic sales, customers, and product data.  
The goal is to demonstrate skills in **Power BI, SQL, and data modeling** applied to a corporate scenario.

---

## 🚀 Features
- **Executive Overview**: Strategic KPIs (Net Sales, Gross Margin, AOV, Orders, Customers).  
- **Sales & Commercial Performance**: Category, channel, and top product analysis.  
- **Customer Analysis (RFM)**: Customer segmentation and ARPU.  
- **Cohort Retention**: Monthly cohort retention matrix and curve.  
- **Financial & Discounts**: Discounts, VAT impact, and profitability metrics.

---

## 🛠️ Tech Stack
- **Power BI** (DAX, Power Query, tabular modeling)  
- **SQL** for fact and dimension table simulation  
- **Excel/CSV** for generating demo datasets  

---

## 📂 Data Structure
- **Fact tables**: `fact_sales`  
- **Dimension tables**: `dim_date`, `dim_customer`, `dim_product`
- **Calculated Tables (support)**:`CohortMonth`,`CohortIndex`,
- **Measure tables (no data rows)**: `Measurements_Basics`,`Measurements_KPI`,`Measurements_Customer`,`Measurements_Cohort`,

---

## Model relationships (chaves)

- **fact_sales[date_key] → dim_date[date_key]
- **fact_sales[customer_id] → dim_customer[customer_id]
- **fact_sales[product_id] → dim_product[product_id]
- **CohortMonth[customer_id] → dim_customer[customer_id] (suporte a coortes)
- **CohortIndex[cohort_month] ↔ usado apenas em medidas/visual de coorte


---

## 📸 Preview
![Sales View](assets/preview.png)  
![Financial View](assets/preview2.png)
---

## 🎯 Key Learnings
- Applied **cohort analysis** for retention.  
- Built **financial measures** (Gross Margin, Discount %, Net Sales).  
- Corporate-style layout applicable to real retail companies.  

---

## 📥 File
- [Download Dashboard PDF](./NovaEra_Retail_Demo.pdf)

---

## 👨‍💻 Author
**Leonardo Cabral** – Data Analyst | Power BI | SQL | SAP | Power Platform  
Certification in progress: **Microsoft PL-300**
