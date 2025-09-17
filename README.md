# Online Banking Dashboard

Welcome! This repository holds a Power BI dashboard I've created for analyzing online banking data. The goal is to turn raw data into clear, actionable insights for tracking customer behavior, transaction trends, and key performance indicators.

## How It Works: My Data Pipeline

This project uses a simple but effective data pipeline, which is a lot like a digital factory for data.

* **Extraction:** The process starts by pulling data from source files, like Excel spreadsheets, where the raw customer and transaction data lives.
* **Transformation:** Next, I get the data ready for analysis. This involves cleaning it up and structuring it in a relational database. For example, I connect customer information to their transaction history.
* **Loading:** Finally, the clean, structured data is loaded into Power BI's data model, where I can build all the visualizations you see on the dashboard.

## Tools I Used

I used a few key tools to bring this project to life:

* **MySQL Workbench 8.0 CE & DBeaver:** These are my go-to tools for managing databases. I used them to create the database, build the tables, and run the SQL queries that calculate all the key metrics.
* **Power BI:** This is where the magic happens! I used it to connect to the database, model the data, and design the interactive dashboard that tells the story behind the numbers.

## Getting Started with the Project

If you want to explore this project or use it yourself, here's how to get it running:

1.  **Set up the Database:** Open either MySQL Workbench or DBeaver. Create a new database called `online_banking`.
2.  **Create Tables & Import Data:** Run the `CREATE TABLE` scripts to set up the necessary tables. Then, use the import wizard in your database tool to load your data from the source files into the `customer_joining_info` and `customer_transactions` tables.
3.  **Connect in Power BI:** Open the `Online_Banking_Dashboard.pbix` file. You'll need to update the data source settings to connect to your MySQL database. Just enter your credentials, and you're all set!
4.  **Refresh the Data:** Once you've connected, click "Refresh" in the Power BI ribbon to pull all the data from your database into the dashboard.

## A Look at the Dashboard Visuals

The dashboard is designed to be intuitive and easy to navigate. Here's a quick breakdown of what each section tells you:

* **KPI Cards:** The cards at the top show **Total Customers** and **Total Closing Balance**. They're the most important numbers, giving you an instant overview of the bank's size and financial health.
* **Regional & Area Breakdown:** These bar and donut charts show where customers are located. They're great for spotting which regions are driving growth and where to focus marketing efforts.
* **Financial Trends:** The line chart tracking **Monthly Closing Balance** is a powerful visual. It helps you see how the bank's finances are changing over time, revealing seasonal patterns or periods of rapid growth.
* **Transaction Activity:** Charts comparing **Deposits vs. Withdrawals** and showing **Weekly Deposit Trends** give a clear picture of cash flow and customer engagement. You can see how active customers are and how consistent deposits are over time.
