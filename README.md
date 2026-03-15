# 📦 FedEx Logistics Performance Analysis (EDA)

## 📌 Project Overview

This project performs **Exploratory Data Analysis (EDA)** on a logistics dataset related to **FedEx global supply chain operations**. The goal of the analysis is to identify patterns affecting **delivery performance, shipment reliability, vendor efficiency, and logistics costs**.

By analyzing shipment data such as shipment mode, country, vendor information, delivery timelines, shipment weight, freight cost, and insurance cost, the project uncovers insights that can help optimize supply chain operations.

The analysis helps answer key business questions such as:

* What factors affect **on-time delivery**?
* Does **shipment mode** impact delivery performance?
* Which **countries experience more delivery delays**?
* Does **vendor lead time affect delivery reliability**?
* Is there a relationship between **shipment weight and insurance cost**?

The insights generated from this analysis can support **data-driven decision making in logistics planning and supply chain management**.

---

# 🎯 Business Objective

The primary objective of this project is to **improve supply chain efficiency and delivery reliability** by identifying the factors influencing shipment delays and logistics costs.

Key goals include:

* Improve **on-time delivery performance**
* Identify **high-delay regions and vendors**
* Understand **cost drivers such as freight and insurance**
* Support **better shipment planning and vendor selection**

---

# 📊 Dataset Information

The dataset contains **10,000+ logistics shipment records** with **33 features** including shipment details, product information, delivery dates, and cost metrics.

### Important Features

| Feature                   | Description                                                     |
| ------------------------- | --------------------------------------------------------------- |
| Country                   | Destination country of shipment                                 |
| Managed By                | Team responsible for logistics management                       |
| Shipment Mode             | Transportation mode (Air, Sea, Truck, etc.)                     |
| Vendor INCO Term          | International commercial terms defining shipment responsibility |
| Scheduled Delivery Date   | Planned delivery date                                           |
| Delivered to Client Date  | Actual delivery date                                            |
| Weight (Kilograms)        | Weight of shipment                                              |
| Freight Cost (USD)        | Shipping cost                                                   |
| Line Item Insurance (USD) | Insurance cost for shipment                                     |

---

# 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Google Colab / Jupyter Notebook

---

# 🔧 Data Cleaning & Preprocessing

The following steps were performed to prepare the dataset for analysis:

* Removed spaces and special characters from column names
* Handled missing values
* Converted relevant columns to numeric format
* Converted date columns to datetime format
* Removed extreme outliers
* Created new derived features

### Feature Engineering

Three important new features were created:

**Delivery Delay Days**

```
Delivery Delay Days = Delivered Date - Scheduled Delivery Date
```

**On-Time Delivery Flag**

```
On Time = 1 if Delivery Delay <= 0 else 0
```

**Vendor Lead Time**

```
Vendor Lead Time = Scheduled Delivery Date - PO Sent to Vendor Date
```

These features helped analyze shipment performance more effectively.

---

# 📈 Exploratory Data Analysis

Several visualizations were created to understand relationships between variables.

## 1️⃣ Team Performance Analysis

A bar chart was used to compare **on-time delivery performance across logistics teams**.

**Insight**

* Some teams consistently achieve higher on-time delivery rates.

---

## 2️⃣ Shipment Mode vs Delivery Performance

A count plot was used to analyze **on-time vs delayed deliveries across shipment modes**.

**Insight**

* Shipment mode significantly affects delivery reliability.
* Air shipments tend to have higher on-time rates.

---

## 3️⃣ Country-Wise Delivery Delay Analysis

A bar chart identified countries with the **highest average delivery delays**.

**Insight**

* Certain countries show consistent delays, possibly due to customs or infrastructure challenges.

---

## 4️⃣ Vendor Lead Time vs Delivery Outcome

A boxplot was used to compare **vendor lead times for on-time vs delayed shipments**.

**Insight**

* Longer vendor lead times increase the likelihood of shipment delays.

---

## 5️⃣ INCO Terms and Vendor Performance

A line chart analyzed **on-time delivery percentage across different INCO terms**.

**Insight**

* Some INCO terms result in better delivery reliability than others.

---

## 6️⃣ Weight vs Insurance Cost

A scatter plot with regression was used to analyze **relationship between shipment weight and insurance cost**.

**Insight**

* Insurance cost generally increases with shipment weight.

---

## 7️⃣ Correlation Analysis

A correlation heatmap was used to analyze relationships between numerical variables.

**Key Findings**

* Strong correlation between **Line Item Quantity and Line Item Value**
* Positive correlation between **Weight and Freight Cost**
* Moderate correlation between **Shipment Value and Freight Cost**

---

# 📊 Key Insights

* Shipment mode has a significant impact on delivery performance.
* Vendor lead time is a major contributor to shipment delays.
* Some countries consistently experience higher delivery delays.
* Heavier shipments lead to higher freight and insurance costs.
* Shipment quantity strongly influences total shipment value.

---

# 💡 Business Recommendations

Based on the analysis, the following recommendations were proposed:

### 1️⃣ Optimize Shipment Mode

Use air shipments only for urgent deliveries and shift heavy shipments to sea or truck to reduce costs.

### 2️⃣ Improve Vendor Monitoring

Track vendors with long lead times and renegotiate contracts if necessary.

### 3️⃣ Country-Specific Logistics Planning

Implement buffer times for shipments to high-delay countries.

### 4️⃣ Freight Cost Optimization

Consolidate shipments and negotiate freight contracts to reduce shipping expenses.

### 5️⃣ Data-Driven Logistics Planning

Use predictive models to forecast shipping costs and delivery delays.

---

# 📌 Conclusion

This project demonstrates how **data analysis can improve supply chain efficiency** by identifying patterns affecting delivery performance and logistics costs.

Through exploratory data analysis and visualization, the project highlights opportunities for **better shipment planning, vendor management, and cost optimization**.

---

# 👨‍💻 Author

**Pamendra Kaushik**

Data Analyst | Python | SQL | Data Visualization

---
