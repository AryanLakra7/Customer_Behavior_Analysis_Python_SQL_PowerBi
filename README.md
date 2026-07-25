# 🛍️ Customer Shopping Behavior Analysis

## 📌 Project Overview

This project focuses on analyzing customer shopping behavior using data analytics, SQL, and visualization tools. The goal is to uncover patterns in customer purchases, demographics, and engagement to support data-driven business decisions.

The project integrates:

* **Python (Pandas)** for data cleaning and preprocessing
* **SQL (PostgreSQL)** for structured data analysis
* **Power BI** for interactive dashboard visualization

---

## 📂 Project Structure

```
├── customer_shopping_behavior_analysis.ipynb   # Data cleaning & preprocessing (Python)
├── customer_behavior_analysis.sql             # SQL queries for analysis
├── customer_behavior_dashboard.pbix           # Power BI dashboard
├── customer_shopping_behavior.csv             # Dataset (not included here)
└── README.md                                  # Project documentation
```

---

## ⚙️ Data Processing (Python)

The dataset was cleaned and transformed using Pandas:

### Key Steps:

* Loaded dataset using `pandas`
* Handled missing values:

  * Filled missing **Review Ratings** using median values grouped by category
* Standardized column names:

  * Converted to lowercase
  * Replaced spaces with underscores
* Renamed columns for consistency
* Feature engineering:

  * Created **age groups** using quartiles:

    * Young Adult, Adult, Middle Aged, Senior
  * Converted purchase frequency into numeric days
* Removed redundant columns (e.g., `promo_code_used`)

---

## 🗄️ Database Integration (SQL)

* Data was stored in a **PostgreSQL database**
* Connection established using:

  * `SQLAlchemy`
  * `psycopg2`
* SQL scripts were used to:

  * Perform aggregations
  * Analyze customer segments
  * Generate business insights

---

## 📊 Power BI Dashboard

The `.pbix` file contains an interactive dashboard with:

### Key Visualizations:

* Customer demographics analysis (Age groups, Gender)
* Purchase behavior trends
* Category-wise sales distribution
* Impact of discounts on purchases
* Frequency of purchases insights

---

## 🔍 Key Insights (Sample)

* Customer purchasing patterns vary significantly across age groups
* Discounts influence buying behavior
* Certain product categories drive higher revenue
* Purchase frequency correlates with customer segmentation

---

## 🛠️ Tech Stack

* **Python**: Pandas, NumPy
* **Database**: PostgreSQL
* **Libraries**: SQLAlchemy, psycopg2
* **Visualization**: Power BI

---

## 🚀 How to Run

### 1. Python Analysis

```bash
pip install pandas sqlalchemy psycopg2-binary
```

Run the notebook:

```bash
jupyter notebook customer_shopping_behavior_analysis.ipynb
```

---

### 2. Database Setup

* Install PostgreSQL
* Create a database:

```sql
CREATE DATABASE customer_behavior;
```

* Update credentials in notebook:

```python
username = "postgres"
password = "your_password"
host = "localhost"
port = "5432"
database = "customer_behavior"
```

---

### 3. Power BI Dashboard

* Open `.pbix` file in Power BI Desktop
* Refresh data connection if needed

---


## 👨‍💻 Author

**Aryan Lakra**
B.Tech – Production & Industrial Engineering

