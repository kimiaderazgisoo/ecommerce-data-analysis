# 🛒 E-Commerce Business Intelligence Dashboard

An end-to-end **E-Commerce Business Intelligence project** built to transform synthetic e-commerce data into meaningful business insights using **Python, SQL Server, and Power BI**.

The project covers the complete workflow from **data generation and validation** to **database integration, data modeling, and interactive dashboard development**.

---

## 📌 Project Overview

The goal of this project was to build a realistic e-commerce analytics environment and develop an interactive Business Intelligence dashboard for exploring business, customer, and product performance.

The dataset was generated from scratch using **Python and Faker**, validated using multiple data-quality checks, stored in **SQL Server**, and finally connected to **Power BI** for analysis and visualization.

### End-to-End Workflow

```text
Python + Faker
      ↓
Data Generation
      ↓
Data Validation
      ↓
SQL Server Database
      ↓
Data Modeling
      ↓
Power BI
      ↓
Interactive Dashboard
      ↓
Business Insights
```

---

## 🎯 Business Objectives

The project focuses on answering key business questions such as:

* How is the overall business performing?
* How are customer numbers changing over time?
* What percentage of customers are repeat customers?
* Where are customers geographically distributed?
* Which products generate the most revenue?
* Which product categories perform best?
* How many units are being sold?
* What are the key customer and product performance indicators?

---

# 🐍 Data Generation with Python

The e-commerce dataset was generated programmatically using **Python** and the **Faker** library.

The dataset was designed to simulate realistic e-commerce entities and relationships, including customers, products, orders, and order-related information.

The data-generation and loading process is implemented in a **Jupyter Notebook (`.ipynb`)**.

### Python Libraries

* **Pandas** — Data manipulation and DataFrame operations
* **NumPy** — Numerical operations
* **Faker** — Generation of realistic synthetic data
* **Random** — Randomized data generation
* **Datetime** — Date and time generation
* **TQDM** — Progress tracking

---

# ✅ Data Validation

Because the dataset was generated synthetically, several validation methods were applied before loading the data into the database.

The generated data was checked for issues including:

* Missing or null values
* Duplicate records
* Invalid relationships between tables
* Incorrect data types
* Inconsistent values
* Data integrity issues

This step helped ensure that the generated dataset was sufficiently consistent and reliable for analytical use.

---

# 🗄️ SQL Server Integration

After generating and validating the data, a relational database was created in **SQL Server**.

The Jupyter Notebook establishes a connection to the SQL Server database using the configured database parameters and loads the validated datasets into the corresponding tables.

### Data Loading Workflow

```text
Generate Data
     ↓
Validate Data
     ↓
Connect to SQL Server
     ↓
Load Data into Tables
     ↓
Verify Database Data
```

---

# ⚙️ Installation & Configuration

## 1. Clone the Repository

Clone this repository to your local machine:

```bash
git clone https://github.com/kimiaderazgisoo/ecommerce-data-analysis.git
cd your-repository
```

---

## 2. Install Python Dependencies

The required Python packages are listed in `requirements.txt`.

Install them using:

```bash
pip install -r requirements.txt
```

---

## 3. Configure Environment Variables

Database connection parameters are stored using environment variables rather than being hard-coded into the notebook.

First, create your `.env` file from the provided `.env.example`:

```bash
cp .env.example .env
```

Then open `.env` and configure your SQL Server connection parameters.

Example:

```text
DB_SERVER=your_server_name
DB_NAME=your_database_name
DB_USER=your_username
DB_PASSWORD=your_password
```

> **Important:** The `.env` file contains local database configuration and credentials. Do not commit it to GitHub.

The `.env.example` file is included in the repository as a template.

---

## 4. Prepare SQL Server

Create the required database and tables in SQL Server before running the data-loading workflow.

The database is used as the central storage layer between the Python data-generation process and Power BI.

---

## 5. Run the Jupyter Notebook

Open the Jupyter Notebook included in the repository using Jupyter Notebook or JupyterLab.

The notebook performs the following steps:

1. Generates the synthetic e-commerce dataset.
2. Validates the generated data.
3. Establishes a connection to SQL Server.
4. Loads the datasets into the corresponding database tables.

---

# 🔗 Power BI Integration

Once the data has been loaded into SQL Server, the database is connected to **Power BI**.

The Power BI model contains the required relationships between the tables and provides the foundation for creating analytical measures and interactive visualizations.

**SQL Server → Power BI → Data Model → DAX Measures → Visualizations**

---

# 📊 Dashboard

The current version of the project contains three main Power BI pages:

### 1. Overview

Provides a high-level view of business performance, including:

* Key Performance Indicators
* Revenue trends
* Customer segmentation
* Customer distribution
* Overall business performance

![Overview Dashboard](https://github.com/kimiaderazgisoo/ecommerce-data-analysis/blob/main/screenshots/01-Overview.png)

---

### 2. Customer Analysis

Focuses on customer behavior and characteristics, including:

* Total Customers
* New Customers
* Repeat Customers
* Customer Growth
* Repeat Customer Rate
* Active Customer Rate
* Customer Age Distribution
* Customer Segmentation
* Geographic Distribution

![Customer Analysis Dashboard](https://github.com/kimiaderazgisoo/ecommerce-data-analysis/blob/main/screenshots/02-Customer%20Analysis.png)

---

### 3. Product Analysis

Focuses on product and category performance, including:

* Total Products
* Units Sold
* Average Units per Product
* Product Performance
* Top Products
* Revenue by Category
* Product-level metrics

![Product Analysis Dashboard](https://github.com/kimiaderazgisoo/ecommerce-data-analysis/blob/main/screenshots/03-ProductAnalysis.png)

---

# 🎨 Dashboard Design

The Power BI dashboard was designed with a focus on creating a clean, modern, and visually consistent user experience.

The dashboard backgrounds and visual design assets were created using **Microsoft PowerPoint** and then incorporated into the Power BI report.

---

# 📈 Power BI & DAX

Power BI was used to build the analytical model, create interactive visualizations, and develop business-focused KPIs.

**DAX** was used to create calculated measures for metrics such as:

* Total Customers
* New Customers
* Repeat Customers
* Repeat Customer Rate
* Active Customer Rate
* Total Products
* Units Sold
* Average Units per Product
* Total Revenue
* Average Revenue per Unit
* Product and customer performance metrics

---

# 🔍 Key Insights

The dashboard is designed to help users explore the data from different business perspectives and identify patterns in:

* Customer acquisition and growth
* Customer retention and repeat purchasing
* Geographic customer distribution
* Product performance
* Category performance
* Revenue contribution
* Overall business performance

---

# 🛠️ Tech Stack

| Technology           | Purpose                                       |
| -------------------- | --------------------------------------------- |
| **Python**           | Data generation and validation                |
| **Faker**            | Synthetic data generation                     |
| **Pandas**           | Data manipulation                             |
| **NumPy**            | Numerical operations                          |
| **SQL Server**       | Data storage and database management          |
| **SQL**              | Database operations                           |
| **Power BI**         | Business Intelligence and visualization       |
| **DAX**              | Analytical measures and KPIs                  |
| **PowerPoint**       | Dashboard background and design assets        |
| **Jupyter Notebook** | Data generation and database loading workflow |

---

# 👩‍💻 Author

**Kimia Derazgisoo**

Business Intelligence | Python | SQL | Power BI

---

⭐ If you find this project interesting, feel free to explore the repository and share your feedback.
