📊 Ad Spend Reconciliation Workflow
📌 Project Overview

This repository contains an end-to-end automated pipeline for reconciling Search and Display ad spend across multiple data sources.

The system goes beyond basic reporting by combining:

- Consumption data
- Redemption data
- Credit classifications
- Real-time pacing logic

With the latest update, the project now includes a Tkinter-based ingestion layer, transforming it from a script into a scalable, user-friendly reconciliation tool.

🚀 Key Functionalities

🔄 Data Ingestion (NEW)

    - Multi-file upload via Tkinter UI
    - Supports CSV, XLSX, XLS formats
    - Upload files from multiple folders in one go
    - Eliminates manual file path handling

⚙ Smart File Handling (NEW)

* Rule-based parsing using file names:
    - Skip rows / footers
    - Sheet selection
    - Custom read logic per report
    - Handles inconsistent report formats seamlessly

📦 Centralized Data Management (NEW)

    - All datasets stored in a unified dictionary (dfs)
    - Enables smooth downstream transformations
    - Reduces redundancy and improves pipeline modularity

📥 Data Extraction

* Automated SQL-based extraction of:
    - Consumption reports
    - Redemption reports
    - Ensures consistent and reliable raw data inputs

💰 Financial Segregation

* Automatically classifies ad spend into:
    - Free Credits / Market Credits → Promotional offsets
    - Overburn → Spend exceeding allocated limits
    - Paid Credits → Actual cash outflow
    - Net Spend → Final reconciled spend after adjustments


📊 Reporting & Aggregation

Hierarchical reporting across:

- Business Units (BU)
- Super Categories
* Provides granular visibility into spend behavior

📈 Predictive Pacing

* Calculates run-rate based on:
    - Consumed days
    - Remaining days in the month
* Estimates required daily spend to:
    - Stay aligned with monthly budgets
    - Helps ensure month-end accuracy


#⚡ Workflow Overview

1. Data Ingestion
    - Multi-file upload via Tkinter UI
2. Smart Loading
    - Apply file-specific parsing rules
3. Data Normalization
    - Clean, standardize, and map datasets
4. Reconciliation Engine
    - Combine consumption + redemption
    - Apply credit segregation logic
5. Reporting Layer
    - BU & Super Category views
    - Credit breakdown & net spend
6. Insights & Outputs
    - Budget pacing
    - Actionable finance insights

🎯 Impact

⏱  Eliminates manual data preparation

🎯 Improves accuracy via rule-based ingestion

📊 Enables real-time reconciliation visibility

🚀 Shifts focus from data collection → decision making

🔁 Reusable across multiple reporting cycles


🛠 Tech Stack
Python
Pandas
Tkinter (UI Layer)
Jupyter Notebook

