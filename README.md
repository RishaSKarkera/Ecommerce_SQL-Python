# E-commerce Sales & Analytics Pipeline

This project demonstrates a complete data workflow: from raw CSV data ingestion into a relational database (MySQL) to advanced business intelligence analysis and visualization. Using a dataset of e-commerce transactions, the project uncovers insights into customer behavior, sales performance, and payment trends.

## 🚀 Key Features
- **Automated Data Ingestion**: Python script to dynamically create MySQL tables and import data from 7 different CSV sources.
- **Data Cleaning**: Handling missing values (NaNs) and normalizing column headers for SQL compatibility.
- **Advanced SQL Analytics**: Utilizing Joins, Aggregations, Case Statements, and **Window Functions** (DENSE_RANK) to extract deep insights.
- **Data Visualization**: Professional charts generated with Seaborn and Matplotlib to present findings to stakeholders.

## 🛠️ Tech Stack
- **Language**: Python 3.x
- **Database**: MySQL
- **Libraries**: 
    - `Pandas`: Data manipulation and cleaning.
    - `mysql-connector-python`: Database connectivity.
    - `Seaborn` & `Matplotlib`: Statistical data visualization.
    - `NumPy`: Numerical operations.

## 📊 Database Schema
The project utilizes the following relational tables:
- `customers`: Geographic and ID data for buyers.
- `orders`: Purchase timestamps and status.
- `order_items`: Product-level details per order.
- `payments`: Payment values, types, and installment details.
- `products`: Category and physical dimensions of items.
- `sellers`: Seller location and ID details.
- `geolocation`: Latitude/Longitude data for spatial analysis.

## 📈 Analysis Highlights
The notebook performs several high-value business queries:
1. **Sales Performance**: Total revenue calculated per product category.
2. **Customer Demographics**: Count of customers distributed by state and unique cities.
3. **Financial Trends**: Percentage of orders paid via installments vs. full payments.
4. **Top Performers**: Identifying the Top 3 highest-spending customers per year using `DENSE_RANK()` window functions.

## ⚙️ Setup & Installation
1. **Database Setup**: Create a MySQL database named `ecommerce`.
2. **Environment**: Update the `mysql.connector` credentials in the notebook with your local `host`, `user`, and `password`.
3. **Data Path**: Ensure the CSV files are located in the directory specified in the `folder_path` variable.
4. **Run**: Execute the `Ecommerce.ipynb` cells sequentially to build the database and generate the reports.

## 🖼️ Visualizations
The project includes various plots, such as:
- Monthly order distribution.
- Revenue contribution by category.
- Top customer rankings per year.
