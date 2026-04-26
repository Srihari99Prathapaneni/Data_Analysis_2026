__Ad Spend Reconciliation__

📌 Project Overview

This repository contains the end-to-end pipeline for reconciling Search and Display ad spend. The project automates the extraction of consumption and redemption reports, segregates various credit types, and provides month-end estimates to ensure budget adherence across multiple Business Units (BUs).

🚀 Key Functionalities

Automated Extraction: SQL queries designed to pull raw consumption and redemption data.

Financial Segregation: Automatically classifies spend into:
Free Credits / Market Free Credits: Promotional offsets.

Overburn: Spend exceeding allocated limits.

Paid Credits: Actual cash-outflow transactions.

Net Spend: Final spend after all credit adjustments.

Hierarchical Reporting: Aggregates metrics at the Super Category and BU (Business Unit) levels.

Predictive Pacing: Provides run-rate estimates for the remaining days of the current month.
