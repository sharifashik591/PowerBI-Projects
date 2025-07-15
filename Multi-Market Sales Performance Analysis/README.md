
## 📊 Multi-Market Sales Performance Analysis
<img width="1114" height="765" alt="image" src="https://github.com/user-attachments/assets/62c23644-6d99-4c4a-a729-52f78a80ddcc" />


**Tool Used: Power BI | Domain: Retail & Distribution | Year: 2020**

---

### 🧩 **Business Challenge**

In 2020, the organization was managing sales data across multiple regions, customer types, and product lines. However, critical decision-making was hindered by:

* Lack of **consolidated reporting** on revenue and profitability.
* Inability to identify **top-performing markets, customers, or products**.
* No clear visibility into **monthly trends** or **regional contributions**.
* Manual reporting processes consuming valuable time and leading to inconsistent insights.

Leadership needed a centralized, interactive solution to **monitor key sales KPIs**, detect performance patterns, and support data-driven decision-making across departments.

---

### 🎯 **Solution Overview**

As an Advanced Data Analyst, I developed a comprehensive **Sales & Profit Performance Dashboard** in Power BI that enables stakeholders to:

* Monitor overall **sales, revenue, and profit KPIs** at a glance.
* Drill down into performance by **market, product, and customer**.
* Understand revenue contribution by **customer type** and **geographical zones**.
* Track **monthly trends** and visualize **market-wise distribution** on a map.

This solution transformed scattered data into actionable intelligence, reducing manual work and accelerating insight generation.

---

### ⚙️ **Technical Implementation**

#### 1. **Data Ingestion & Preparation**

* Imported and transformed a structured dataset (`transactions_all.csv`) containing \~350K rows of transactional records.
* Cleaned and preprocessed columns such as:

  * `order_date`, `market_name`, `customer_type`, `product_code`, `sales_amount`, `total_profit`, `zone`, etc.
* Extracted additional fields:

  * `Year`, `Month`, `Month Name` using Power Query.

#### 2. **Data Modeling**

* Defined relationships and hierarchies for time-based filtering (`Year`, `Month`).
* Created DAX measures:

  ```DAX
  Total Revenue = SUM(transactions_all[sales_amount])
  Total Profit = SUM(transactions_all[total_profit])
  Total Product Sold = SUM(transactions_all[sales_qty])
  Profit Margin = DIVIDE([Total Profit], [Total Revenue], 0)
  ```
* Added calculated tables and columns to support custom visuals and interactivity.

#### 3. **Interactive Visualization**

Designed a responsive dashboard in Power BI with the following visuals:

| Feature                  | Visualization Type     | Insight Delivered                              |
| ------------------------ | ---------------------- | ---------------------------------------------- |
| Total KPIs               | KPI Cards              | Total product sold, revenue, and profit        |
| Market-Level Performance | Clustered Bar Charts   | Sales, revenue, and profit by region           |
| Monthly Trend Analysis   | Line + Bar Chart Combo | Revenue vs Profit (Jan–Jun 2020)               |
| Top 5 Customers          | Horizontal Bar Chart   | Customer-wise contribution                     |
| Top Products             | Horizontal Bar Chart   | High-performing SKUs                           |
| Revenue by Customer Type | Donut Chart            | E-commerce vs Brick & Mortar revenue share     |
| Revenue by Zone          | Pie Chart              | Zone-wise distribution (North, Central, South) |
| Location Intelligence    | Filled Map / Pie Map   | Market revenue mapped across India             |

#### 4. **User Experience Features**

* Time filters: Slicers for `Year` and `Month` to support trend comparison.
* Dynamic tooltips and interactivity across visuals.
* Clean, modern layout optimized for clarity and decision support.

---

### 📈 **Business Impact**

✅ **Faster Insights:** Reduced reporting time from hours to seconds with a centralized dashboard.
✅ **Strategic Clarity:** Enabled leadership to identify high-value customers, underperforming markets, and optimal product focus.
✅ **Revenue Optimization:** Highlighted top revenue zones and high-margin markets for better resource allocation.
✅ **Cross-Departmental Access:** Shared Power BI dashboards across sales, marketing, and executive teams for unified decision-making.

---

### 💡 **Key Takeaways**

This project demonstrated the power of **data storytelling** through dynamic dashboards and actionable analytics. By bridging raw transactional data with business strategy, I empowered the organization to make **data-backed decisions** with confidence and speed.

---

### 🛠️ **Tools & Skills Used**

* **Power BI Desktop**
* **Power Query M Language**
* **DAX (Data Analysis Expressions)**
* Data Modeling & Normalization
* Data Visualization Best Practices
* Business KPI Design & Executive Reporting

---

Let me know if you'd like an **HTML version**, a **PDF portfolio format**, or help integrating this into your personal website or resume.
