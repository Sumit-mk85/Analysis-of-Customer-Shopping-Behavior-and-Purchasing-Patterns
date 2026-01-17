# Analysis-of-Customer-Shopping-Behavior-and-Purchasing-Patterns
# Overview
This project delivers an end-to-end analysis of consumer shopping habits to identify factors influencing purchasing decisions, segment the customer base, and uncover trends in product popularity. The workflow moves from data extraction and cleaning in Python to structured querying in MySQL, followed by interactive visualization in Power BI, and finally presenting findings via a Gamma-generated deck.

# Dataset
The analysis utilizes a detailed dataset focusing on consumer behavior:
**Volume:** 3,900 rows and 18 columns.
**Key Attributes:**

**Demographics**: Age, Gender, Location, Subscription Status.

**Purchase Details:** Item Purchased, Category, Purchase Amount, Season, Color.

**Behavioral Metrics:** Discount Applied, Frequency of Purchases, Previous Purchases, Review Rating.


# Tools & Technologies
**Python (Pandas):** Data loading, cleaning, missing value handling, and feature engineering.

**MySQL:** Relational database management and structured business logic queries.

**Power BI:** Interactive dashboard creation and data visualization.

**Gamma:** Presentation and storytelling.

# Steps Involved
**1. Data Cleaning & Engineering (Python)**

  **Data Loading:** Loaded raw CSV data using Pandas.

  **Handling Missing Values:** Imputed null values in 'Review Rating' using the median rating grouped by category.

  **Standardization:** Renamed columns to snake_case for consistency (e.g., purchase_amount).

  **Feature Engineering:** Created new attributes such as age_group and purchase_frequency_days .

  **Database Integration:** Connected Python to MySQL Workbench to load the cleaned data.

**2. Data Analysis (SQL)**
Executed structured SQL queries to extract key business insights:

**Revenue Analysis:** Calculated revenue distribution by gender and age group.

**Customer Segmentation:** Categorized users into 'New', 'Returning', and 'Loyal' segments based on purchase history .

**Product Performance**: Identified top-rated products and high-volume categories.

**Shipping & Subscription:** Analyzed average spending differences between subscribers and non-subscribers.

**3. Visualization (Power BI)**
Built an interactive "Customer Behavior Dashboard" to visualize KPIs:

**Key Metrics Displayed:** 
**Total Customers (3.9K), Average Purchase Amount ($59.76), and Average Review Rating (3.76)** .

**Visuals:**

**Sales & Revenue by Category (Clothing, Accessories, Footwear).**

**Revenue by Age Group (Youth, Middle Age, Senior).**

**Subscription Distribution (27% Subscribers vs. 73% Non-Subscribers).**

**4. Reporting**
Generated a comprehensive report and utilized Gamma to create a slide deck summarizing the business recommendations.

Dashboard
The dashboard provides a high-level view of customer demographics and sales performance. (Note: Detailed interactive views are available in the .pbix file)

# Key Results & Insights

**Demographic Revenue Gap:** Male customers generated **$157,890** in revenue, significantly outperforming female customers ($75,191).

**Customer Loyalty:** The majority of the customer base falls into the "Loyal" segment (3,116 customers), while new customer acquisition remains low (83 customers).

**Subscription Value:** Subscribers have a slightly lower average spend ($59.49) compared to non-subscribers ($59.87), indicating a need to revamp the subscription value proposition.

**Top Products:** "Hat" and "Sneakers" are the highest purchased products when discounts are applied.

# How to Run
Clone the Repository:

**Python Processing:**

Install dependencies: pip install pandas mysql-connector-python

Run the cleaning script to generate the clean dataset and upload it to MySQL.

**SQL Analysis:**

Import the cleaned data into your MySQL instance.

Run the provided .sql scripts to replicate the analysis metrics.

**Dashboard:**

Open customer_shopping_behavior.pbix in Power BI Desktop.

Ensure the data source settings point to your local MySQL database.
