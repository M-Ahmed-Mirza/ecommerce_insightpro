# 🛒 E-Commerce InsightPro

An end-to-end e-commerce analytics platform that segments customers using **RFM (Recency, Frequency, Monetary) analysis**, powered by a Python-based **ETL pipeline** from SQL Server to Power BI, with interactive dashboards embedded in a Flask web application.

---

## The Problem

E-commerce businesses sit on mountains of transaction data but often lack the tools to turn it into actionable insights. Questions like *"Who are our most valuable customers?"*, *"Which customers are about to churn?"*, and *"Where should we focus our marketing spend?"* require structured analysis — not just raw sales reports.

## The Solution

E-Commerce InsightPro answers these questions through a three-layer architecture:

1. **ETL Pipeline** — Extracts raw transaction data from SQL Server, transforms it (cleaning, aggregation, feature engineering), and loads the processed data into Power BI datasets.
2. **RFM Segmentation** — Scores every customer on Recency (how recently they purchased), Frequency (how often they purchase), and Monetary value (how much they spend), then assigns them to segments like *Champions*, *Loyal Customers*, *At Risk*, and *Lost*.
3. **Interactive Dashboard** — Power BI dashboards embedded inside a Flask web application, giving stakeholders a single URL to explore customer segments, track trends, and make data-driven decisions.

---

## Tech Stack

| Layer              | Technology                          |
|--------------------|-------------------------------------|
| ETL & Data Processing | Python, Pandas, NumPy            |
| Database           | SQL Server                          |
| Analytics          | RFM Segmentation, Customer Scoring  |
| Visualization      | Power BI (embedded)                 |
| Web Application    | Flask, HTML, CSS                    |
| Dataset            | Real e-commerce transaction data    |

---

## RFM Segmentation

Customers are scored on three dimensions:

| Dimension   | What It Measures                        | Score Range |
|-------------|----------------------------------------|-------------|
| **Recency** | Days since last purchase               | 1–5         |
| **Frequency** | Total number of purchases            | 1–5         |
| **Monetary** | Total amount spent                    | 1–5         |

These scores combine to create customer segments:

| Segment             | Description                                      |
|---------------------|--------------------------------------------------|
| 🏆 Champions        | Recent, frequent, high-spending buyers            |
| 💎 Loyal Customers  | Consistent repeat buyers                          |
| ⚠️ At Risk          | Previously active, now slowing down               |
| 💤 Lost             | Haven't purchased in a long time                  |

---

## Project Structure

```
ecommerce_insightpro/
├── app/                    # Flask web application
├── fonts/                  # Custom fonts for the dashboard UI
├── resources/img/          # Images and visual assets
├── samples/                # Sample data files
├── run.py                  # Application entry point
├── .env.example            # Environment variables template
├── requirements.txt        # Python dependencies
└── README.md
```

---

## Getting Started

### Prerequisites

- Python 3.8+
- SQL Server instance with the e-commerce dataset loaded
- Power BI account (for embedded dashboards)

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/M-Ahmed-Mirza/ecommerce_insightpro.git
cd ecommerce_insightpro

# 2. Install dependencies
pip install -r requirements.txt

# 3. Set up environment variables
cp .env.example .env
# Edit .env with your SQL Server and Power BI credentials

# 4. Run the application
python run.py
```

---

## Key Features

- **Automated ETL Pipeline** — Extracts data from SQL Server, cleans and transforms it, and pushes processed datasets to Power BI with minimal manual intervention.
- **Customer Segmentation** — RFM-based scoring that groups customers into actionable segments for targeted marketing strategies.
- **Embedded Dashboards** — Power BI visuals embedded directly in the Flask app so stakeholders can explore data without needing a Power BI license.
- **Web-Based Access** — Single URL access for the team — no installation required for end users.

---

## Screenshots

> *Screenshots of the dashboard coming soon.*

---

## Dataset

This project uses a real-world e-commerce transaction dataset. The ETL pipeline is designed to work with any transactional dataset that includes customer IDs, purchase dates, and transaction amounts.

---

## Author

**Muhammad Ahmed Mirza**  
AI Engineer | [LinkedIn](https://www.linkedin.com/in/muhammad-ahmed-mirza-4282a726b) | [GitHub](https://github.com/M-Ahmed-Mirza)
