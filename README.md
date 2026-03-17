# Supply Chain Delivery Performance & Risk Analysis

## 📈 Executive Summary
In global logistics, delivery performance is the primary driver of customer retention and cost control. This project provides a diagnostic analysis of 1,200 shipment records to identify operational bottlenecks and quantify the financial impact of delivery failures.

**The Outcome:** A strategic dashboard that moves beyond simple reporting to provide prescriptive insights into regional performance gaps and carrier reliability, identifying over **$1.8M in revenue currently at risk.**

---

## 🎯 Project Objectives
* **Quantify Performance:** Identify regional variance against the **85% On-Time Delivery (OTD) target**.
* **Identify Root Causes:** Isolate the primary drivers of delays (e.g., Weather vs. Inventory Holds).
* **Financial Risk Assessment:** Calculate the **Order Value at Risk** to prioritize operational interventions.
* **Carrier Benchmarking:** Compare Actual vs. Planned transit times across major carriers.

---

## 🛠️ Technical Implementation
* **Data Modeling:** Implemented a **Star Schema** to separate shipment facts from dimension tables (Calendar, Geography, Carriers), ensuring model scalability and performance.
* **Power BI UI/UX:** Built an executive-grade interface utilizing a **60%–80% truncated axis** to highlight regional performance gaps and **Gauge visuals** for real-time KPI tracking.
* **Advanced DAX:** Developed complex measures for **On-Time Rate %**, **Month-over-Month (MoM) Trend**, and **Revenue at Risk** calculations.
* **Data Transformation:** Performed ETL in Power Query to normalize date formats and handle null values in delay categorization.

---

## 💡 Key Operational Insights
* **The Regional Gap:** While the overall delay rate is 20.25%, Western provinces (BC/Manitoba) show significantly higher volatility, consistently failing to meet OTD targets due to geographic transit constraints.
* **High-Value Exposure:** Late deliveries currently impact **$1.8M in total order value**, highlighting a critical need for localized buffer-stocking strategies.
* **Carrier Efficiency:** Analysis revealed that Canada Post averages **0.4 days more in transit** than FedEx, contributing to SLA breaches in 15% of Ground-mode shipments.

---

## 🚀 Strategic Recommendations
* **Carrier Optimization:** Shift high-priority Western region shipments to FedEx to mitigate the 0.4-day transit lag.
* **Inventory Buffering:** Increase safety stock levels in Vancouver and Calgary during peak weather months to offset the 21.4% delay rate attributed to environmental factors.
* **Warehouse Process Review:** With **Inventory Holds (25.1%)** being the leading delay reason, a lean audit of warehouse release protocols is recommended to reduce internal dwell time.

---

## 📊 Data Dictionary
The analysis is based on the `supply_chain_dataset_pandora.csv` which includes:
* **Planned vs. Actual Transit Days:** Used to calculate carrier efficiency.
* **On_Time_Flag:** Binary indicator used as the primary performance KPI.
* **Order_Value_CAD:** Financial metric used to weigh the severity of operational delays.

---

## 📬 Contact
* **Name:** Pandora Wong
* **LinkedIn:** [www.linkedin.com/in/pandora-wong]
