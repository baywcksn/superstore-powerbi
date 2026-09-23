# E-Commerce Sales Analytics — Power BI

Interactive e-commerce sales analytics dashboard built with Microsoft Power BI using the Superstore dataset.

The project focuses on analyzing sales performance, profitability, order volume, sales trends, and category performance through an interactive dashboard.

## Dashboard Preview
<img width="6150" height="3525" alt="Superstore_Sales_Analytics_Dashboard" src="https://github.com/user-attachments/assets/8f0cd8bd-c02c-459c-9afe-fa7e03ba2030" />


## Business Questions

This project answers several business questions:

- What is the total sales generated?
- What is the total profit generated?
- How many orders were placed?
- How does sales performance change over time?
- Which product category generates the most sales?
- Which product category generates the most profit?

## Dashboard

The dashboard contains:

- **Total Sales**
- **Total Profit**
- **Total Orders**
- **Monthly Sales Trend**
- **Sales by Category**
- **Profit by Category**
- **Region Filter**
- **Category Filter**

Users can interact with the dashboard using the available filters to analyze different regions and product categories.

## Data Preparation

The dataset was prepared using **Power Query** in Power BI.

Main data preparation steps included:

- Reviewing column data types
- Changing Postal Code from numeric to text
- Checking data quality
- Checking duplicate Row IDs
- Checking invalid sales and quantity values
- Validating order and shipping dates
- Trimming text values in Category and Sub-Category

## Data Model

The project currently uses one main table:

**Fact_Orders**

Key fields include:

- Order ID
- Order Date
- Ship Date
- Customer
- Segment
- Region
- Product
- Category
- Sub-Category
- Sales
- Quantity
- Discount
- Profit

## DAX Measures

The dashboard uses the following DAX measures:

```DAX
Total Sales = SUM(Fact_Orders[Sales])

Total Profit = SUM(Fact_Orders[Profit])

Total Orders = DISTINCTCOUNT(Fact_Orders[Order ID])
```

## Tools

- **Microsoft Power BI**
- **Power Query**
- **DAX**
- **Microsoft Excel**
- **GitHub**

## Dataset

The project uses the **Superstore Dataset** for educational and portfolio purposes.

**Source:** [Superstore Dataset — Kaggle](https://www.kaggle.com/datasets/divyjn28/superstore-dataset)

The dataset contains e-commerce order information including customers, products, categories, regions, sales, discounts, and profits.

## Project Structure

```text
superstore-powerbi/
│
├── dashboard/
│   ├── E-Commerce_Sales_Analytics.pbix
│   └── E-Commerce_Sales_Analytics.pdf
│
├── images/
│   └── dashboard-preview.png
│
└── README.md
```

## Project Status

**Completed — Version 1**

The current version focuses on basic sales and profitability analysis.

Future improvements may include:

- Customer analysis
- Product-level analysis
- Regional performance analysis
- Discount analysis
- Year-over-year performance
- Additional business insights

## Author

**Bayu Wicaksono**

Data Analytics Portfolio Project
