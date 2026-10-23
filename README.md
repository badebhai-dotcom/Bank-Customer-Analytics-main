# Bank-Customer-Analytics-main
# 💳 Fintech Transaction & User Onboarding Analytics Dashboard

![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Excel](https://img.shields.io/badge/Excel-217346?style=for-the-badge&logo=microsoftexcel&logoColor=white)
![DAX](https://img.shields.io/badge/DAX-Data_Analysis_Expressions-orange?style=for-the-badge)

An end-to-end Power BI analytics project designed to track financial transaction performance, evaluate payment channel reliability, and optimize user onboarding and KYC conversion funnels.

---

## 📌 Executive Summary
In modern digital banking and fintech environments, tracking transaction health and customer onboarding friction is critical for revenue retention and regulatory compliance. This project delivers an executive dashboard tracking the full customer lifecycle—from initial app download and wallet setup to full KYC completion—while providing granular diagnostic visibility into payment failure modes across diverse transaction channels.

---

## 🖥 Dashboard Architecture

### Page 1: Financial Transaction Performance
* **Transaction Volume & Velocity:** Real-time visibility into transaction throughput across payment modes (UPI, Credit/Debit Cards, Net Banking, Wallets).
* **Payment Channel Diagnostics:** Evaluates transaction success and failure ratios to isolate channel-level bottlenecks.
* **Failure Pattern Root Cause:** Analyzes technical drop-offs, gateway time-outs, and insufficient fund errors to support payment infrastructure stability.

### Page 2: User Onboarding & KYC Analytics
* **Conversion Funnel Tracking:** Maps user journey attrition across four milestone stages:
  $$\text{App Download} \longrightarrow \text{User Activation} \longrightarrow \text{Wallet Activation} \longrightarrow \text{Full KYC}$$
* **Verification Pipeline Diagnostics:** Monitors drop-off velocity during identity/document verification stages.
* **Cohort Drop-off Analysis:** Identifies user friction points to support product re-engineering and improve KYC completion rates.

---

## 🛠 Tech Stack & Skills
* **Business Intelligence:** Power BI Desktop
* **Data Processing & Modeling:** Power Query (M), Star Schema Architecture
* **Advanced Analytics:** DAX (Data Analysis Expressions) for Time Intelligence, Funnel Conversion %, Failure Rate %, and Dynamic KPI cards
* **Data Source:** Excel / Tabular Financial Records

---

## 📐 Key DAX Measures Implemented
* **Transaction Success Rate (%):**
  $$\text{Success Rate} = \frac{\text{Total Successful Transactions}}{\text{Total Transactions Initiated}} \times 100$$
* **Stage-by-Stage Funnel Conversion (%):**
  $$\text{Funnel Conversion} = \frac{\text{Users at Stage } n}{\text{Users at Stage } (n-1)} \times 100$$
* **Failure Ratio by Channel:**
  $$\text{Channel Failure \%} = \frac{\text{Failed Transactions in Channel}}{\text{Total Transactions in Channel}} \times 100$$

---

## 📂 Repository Structure
```text
├── data/
│   └── Fintech_Data.xlsx               # Source financial dataset
├── reports/
│   └── Fintech_Dashboard.pbix          # Interactive Power BI report file
├── assets/
│   ├── dashboard_1_preview.png         # Transaction Performance screenshot
│   └── dashboard_2_preview.png         # Onboarding & KYC screenshot
└── README.md                           # Documentation
