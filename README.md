# Welder Performance & Quality Analytics Dashboard

## 📌 Project Overview
In heavy manufacturing and fabrication, tracking welding defects is critical for structural integrity and cost control. This project provides a business intelligence dashboard designed to monitor Welder Performance and analyze Defect Per Unit (DPU) metrics. 

By synthesizing data from shop-floor inspection reports and Non-Destructive Testing (NDT) logs, this dashboard allows quality engineering teams to move away from static spreadsheets and make real-time, data-driven decisions regarding operator training and process optimization.

## 🛠️ Tech Stack
* **Data Visualization:** Power BI
* **Data Transformation:** Power Query / DAX
* **Database/Storage:** SQL / Excel (Inspection Logs)

## 📊 Key Features & Business Impact

* **Method vs. Man DPU Analysis:** A critical feature that separates systemic process issues ("Method") from individual operator errors ("Man"). This prevents misdirected training efforts and highlights when a specific welding procedure specification (WPS) needs review.
* **Granular Defect Tracking:** Tracks specific defect typologies (e.g., Crater Pipe, Weld Undercut, Incomplete Penetration). By categorizing defects accurately—accounting for specific process limitations like solid MIG wire characteristics—quality teams can quickly identify the root physical causes on the floor.
* **Operator Performance Benchmarking:** Ranks individual operators by overall DPU, allowing floor supervisors to easily identify top performers for complex assemblies and flag operators requiring immediate retraining.
* **Month-over-Month Trend Analysis:** Visualizes temporal defect trends to measure the effectiveness of recently implemented Corrective and Preventive Actions (CAPA).

## 🚀 How to Run the Project
1. Clone this repository to your local machine.
2. Ensure you have Power BI Desktop installed.
3. Open the `Welder_Performance_Dashboard.pbix` file.
4. The dashboard is currently linked to the sample dataset `inspection_logs_sample.csv` included in the `/data` folder. If connecting to a live SQL database, update the data source settings in Power Query.

## 🔮 Future Enhancements
* **Pareto Analysis Integration:** Transitioning pie charts into dynamic Pareto charts to immediately highlight the critical 20% of defects causing 80% of the DPU.
* **Predictive Capability:** Integrating a Python script to forecast potential out-of-control processes based on historical Statistical Process Control (SPC) trends.
* **Live Automated Ingestion:** Connecting the backend to an automated n8n workflow to ingest daily inspection reports directly from floor supervisors via REST API.
