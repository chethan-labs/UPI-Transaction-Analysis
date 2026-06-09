# 💳 UPI Transaction Analysis — Power BI Report

An end-to-end UPI (Unified Payments Interface) analytics project built with **Power BI**, analyzing **20,000 transactions** across multiple banks, cities, payment modes, and purposes.

---

## 📊 Project Overview

This project dives deep into UPI transaction data to surface key insights around:
- Transaction success vs. failure rates
- Payment distribution by purpose (Food, Travel, Shopping, Bill Payment, Others)
- Bank-wise sent & received transaction volumes
- City-level transaction trends
- Device usage — Mobile, Tablet, Laptop
- Payment mode breakdown — Instant vs. Scheduled
- Currency analysis — INR, USD, EUR, GBP
- Customer demographics — Age, Gender

---

## 📁 Repository Structure

```
UPI-Transaction-Analysis/
│
├── UPI_Transactions.xlsx              # Raw dataset (20,000 records, 20 columns)
├── UPI_Transaction_Analysis_Report.pbix  # Power BI report file
├── .gitignore                         # Git ignore rules
└── README.md                          # Project documentation
```

---

## 📋 Dataset Description

**File:** `UPI_Transactions.xlsx`
**Records:** 20,000
**Columns:** 20

| Column | Description |
|---|---|
| `TransactionID` | Unique transaction identifier (TXN00001...) |
| `TransactionDate` | Date of transaction (2024) |
| `TransactionTime` | Time of transaction |
| `Amount` | Transaction amount ($0.05 – $1,999.87) |
| `Currency` | Currency used: INR, USD, EUR, GBP |
| `BankNameSent` | Sender's bank |
| `BankNameReceived` | Receiver's bank |
| `RemainingBalance` | Account balance after transaction |
| `City` | City where transaction occurred |
| `Gender` | Customer gender (Male / Female) |
| `CustomerAge` | Customer age |
| `TransactionType` | Transfer or Payment |
| `Status` | Success or Failed |
| `DeviceType` | Mobile / Tablet / Laptop |
| `PaymentMethod` | Method of payment |
| `PaymentMode` | Instant or Scheduled |
| `MerchantName` | Name of the merchant |
| `Purpose` | Food / Travel / Shopping / Bill Payment / Others |
| `CustomerAccountNumber` | Customer account number |
| `MerchantAccountNumber` | Merchant account number |

### 📈 Key Statistics

| Metric | Value |
|---|---|
| Total Transactions | 20,000 |
| Average Transaction Amount | ~$993.61 |
| Min Transaction Amount | $0.05 |
| Max Transaction Amount | $1,999.87 |
| Transaction Types | 2 (Transfer, Payment) |
| Payment Modes | 2 (Instant, Scheduled) |
| Statuses | 2 (Success, Failed) |
| Purposes | 5 (Food, Travel, Shopping, Bill Payment, Others) |
| Device Types | 3 (Mobile, Tablet, Laptop) |
| Currencies | 4 (INR, USD, EUR, GBP) |

---

## 📊 Power BI Report

**File:** `UPI_Transaction_Analysis_Report.pbix`

The Power BI report includes interactive dashboards covering:

- **Overview Dashboard** — Total transactions, success rate, total amount at a glance
- **Transaction Trends** — Date-wise and time-wise transaction patterns
- **Bank Analysis** — Top sending and receiving banks by volume
- **Purpose Breakdown** — Spending by category (Food, Travel, Shopping, etc.)
- **Device & Payment Mode** — Channel and mode preference analysis
- **Demographic Insights** — Age group and gender-wise transaction behaviour
- **City-Level Analysis** — Geographic distribution of transactions
- **Currency Analysis** — Multi-currency transaction distribution

> 💡 Open with [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free download from Microsoft)

---

## 🚀 Getting Started

### Clone the Repository
```bash
git clone https://github.com/chethan-labs/UPI-Transaction-Analysis.git
cd UPI-Transaction-Analysis
```

### Explore the Data with Python
```python
import pandas as pd

df = pd.read_excel('UPI_Transactions.xlsx')
print(df.shape)           # (20000, 20)
print(df.describe())
print(df['Status'].value_counts())
print(df['Purpose'].value_counts())
```

### Open the Report
1. Download and install [Power BI Desktop](https://powerbi.microsoft.com/desktop/)
2. Open `UPI_Transaction_Analysis_Report.pbix`
3. Explore the interactive dashboards

---

## 🛠️ Tools Used

| Tool | Purpose |
|---|---|
| **Power BI Desktop** | Dashboard creation & interactive visualization |
| **Microsoft Excel (.xlsx)** | Data storage and preparation |
| **Python (pandas)** | Data exploration & validation |

---

## 📌 Key Insights

- 💸 **20,000 transactions** across multiple banks and cities
- 📱 **3 device types** — Mobile, Tablet, and Laptop usage tracked
- 🌍 **4 currencies** — INR, USD, EUR, GBP across international transactions
- 🎯 **5 spending purposes** — Food, Travel, Shopping, Bill Payment, Others
- ✅ **Success vs. Failed** transaction analysis for reliability metrics
- ⚡ **Instant vs. Scheduled** payments split for payment behaviour insights

---

## 👤 Author

**Chethan** — [github.com/chethan-labs](https://github.com/chethan-labs)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
