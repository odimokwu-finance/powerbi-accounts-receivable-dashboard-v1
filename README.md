# Accounts Receivable Dashboard (Power BI)

## Overview
This project is a Power BI dashboard designed to monitor customer receivables, overdue balances, payment status, and collection performance. It provides both an executive summary view and an invoice-level detail view to support cash flow visibility, collections prioritisation, and receivables management.

The dashboard was built as part of a finance analytics portfolio to demonstrate practical Power BI skills relevant to Accounts Assistant, Finance Assistant, and Accounts Receivable roles.

---

## Business Objective
The purpose of this dashboard is to help finance teams:

- track total receivables and cash collections
- monitor outstanding and overdue balances
- identify aging concentration across receivable buckets
- highlight customer-level exposure
- compare receivables against outstanding balances over time
- drill down to invoice-level detail for follow-up and review

---

## Dashboard Pages

### 1. Executive Summary
This page provides a high-level overview of receivables performance through KPI cards, slicers, aging analysis, payment status distribution, customer exposure, and monthly trends.

### 2. Accounts Receivable Invoice Detail
This page provides invoice-level detail, allowing users to review customer balances, invoice dates, due dates, amounts received, outstanding balances, payment status, days overdue, and assigned sales representative.

---

## Key KPIs
The dashboard includes the following core KPIs:

- **Total Receivables**
- **Total Received**
- **Outstanding Amount**
- **Overdue Amount**
- **Collection Rate**
- **Average Collection Days**

These KPIs help assess both the size and quality of the receivables book.

---

## Key Visuals

### Aging Analysis
- **Outstanding Balance by Aging Bucket**
- Buckets used:
  - Current
  - 1–30
  - 31–60
  - 61–90
  - 90+

This visual highlights the concentration of overdue debt and helps identify collections risk.

### Payment Status Analysis
- **Outstanding Balance by Payment Status**
- Statuses used:
  - Paid
  - Partially Paid
  - Open
  - Overdue

This visual shows how outstanding balances are distributed across payment states.

### Customer Exposure
- **Top Customers by Outstanding Balance**

This chart highlights customers with the highest outstanding balances, helping prioritise collections activity.

### Trend Analysis
- **Monthly Receivables vs Outstanding Balance**

This line chart compares invoiced receivables against outstanding balances over time to support trend analysis.

### Invoice Detail
- CustomerName
- InvoiceID
- InvoiceDate
- DueDate
- InvoiceAmount
- AmountReceived
- OutstandingAmount
- PaymentStatus
- DaysOverdue
- SalesRepName

This detail view supports operational review and follow-up.

---

## Data Model
The dashboard was built using a star-schema structure.

### Fact Table
- **Fact_AR_Invoices**

### Dimension Tables
- **DimCustomer**
- **DimDate**
- **DimPaymentStatus**
- **DimSalesRep**

This structure supports clean filtering, reusable measures, and efficient reporting.

---

## DAX Measures
The model includes measures for:

- Total Receivables
- Total Received
- Outstanding Amount
- Overdue Amount
- Collection Rate
- Average Collection Days
- Aging bucket amounts
- Time-intelligence measures such as:
  - Receivables YTD
  - Receivables FYTD
  - Receivables Last Year
  - Receivables YoY %

---

## Key Insight
The dashboard shows that receivables concentration is heavily skewed toward the **90+ day aging bucket**, indicating elevated collection risk and potential pressure on cash flow.

This makes the dashboard useful not only for reporting, but also for identifying where collection focus may be needed.

---

## Screenshots

### Executive Summary
This screenshot shows the main dashboard page with KPI cards, slicers, aging analysis, payment status donut, top customer exposure, monthly trend, and insight statement.

![Executive Summary](images/Executive-Summary.png)

### Aging Chart
This screenshot highlights the aging analysis visual, showing outstanding balances across receivable aging buckets.

![Aging Chart](images/Aging-Chart.png)

### Payment Status Donut
This screenshot shows the payment status distribution of outstanding balances.

![Payment Status Donut](images/Payment-Status-Donut.png)

### Accounts Receivable Invoice Detail
This screenshot shows the invoice-level detail page for operational review and collections follow-up.

![Accounts Receivable Invoice Detail](images/Accounts-Receivable-Invoice-Detail.png)

---

## Files Included
This repository contains:

- `Accounts_Receivable_Dashboard_PowerBI.pbix` — Power BI report file
- source dataset files (CSV / Excel)
- dashboard screenshots
- `README.md`

---

## Tools Used
- **Power BI**
- **DAX**
- **Microsoft Excel / CSV**
- **Star-schema data modelling**

---

## How to Use
1. Download the `.pbix` file from the repository.
2. Open it in Power BI Desktop.
3. If prompted, reconnect the dataset files.
4. Refresh the model.
5. Use slicers to filter by:
   - Region
   - Segment
   - Payment Status
   - Aging Bucket
   - Fiscal Year

---

## Portfolio Relevance
This project demonstrates practical finance reporting capability in:

- Accounts Receivable analysis
- KPI reporting
- Aging analysis
- Customer exposure monitoring
- Payment status analysis
- Invoice-level reporting
- Power BI dashboard design
- DAX measure development
- Data modelling for finance analytics

It is relevant for roles such as:

- Accounts Assistant
- Finance Assistant
- Accounts Receivable Assistant
- Credit Control Assistant
- Finance Analyst (Junior)

---

## Author
**Nwabueze Odimokwu**

Accounting | Finance | Data Analytics

Skills & Technologies:

Power BI • DAX • Excel • Sage 50c • SQL • Python • ACCA

---

## Notes
This project was created for portfolio and learning purposes using sample / practice data.