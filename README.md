🛍️ Customer Shopping Behaviour Analytics
An end-to-end data analytics project exploring retail customer shopping behaviour across 3,900 records and 19 features — from raw data ingestion to interactive dashboards and a presentation-ready report.

📌 Overview
Problem Statement:

"How can a company leverage consumer shopping data to identify trends, improve customer engagement, and optimize marketing and product strategies?"

This project walks through a complete analytics pipeline:

Cleaning and exploring data in Python
Answering business questions with SQL (MySQL)
Visualizing insights in an interactive Power BI Dashboard
Summarizing findings in a structured project report
Presenting results via a Gamma-powered slide deck


📂 Dataset
AttributeDetailSourceCustomer Shopping Behaviour Dataset (CSV)Records3,900 unique customersFeatures19 columnsCategoriesClothing, Footwear, Outerwear, Accessories
Feature Groups:
GroupColumnsDemographicsage, gender, location, age_groupProduct Infoitem_purchased, category, size, color, seasonTransactionpurchase_amount, payment_method, discount_appliedBehaviourprevious_purchases, frequency_of_purchases, purchase_frequency_daysEngagementreview_rating, subscription_status, shipping_type

🛠️ Tools & Technologies
ToolPurposePython (Pandas, NumPy, Matplotlib, Seaborn)Data loading, cleaning, EDA, and visualizationsMySQLStructured querying to answer 10 business questionsPower BI DesktopInteractive dashboard for KPIs and segment insightsGammaAI-powered presentation slide deckWord / PDFDetailed project report

🔄 Project Steps
1. 🐍 Data Loading & Cleaning (Python)

Loaded the raw CSV dataset using pandas
Removed duplicate records and handled missing values
Standardised column formats and corrected data types
Engineered two new features:

age_group — categorised customers into age brackets
purchase_frequency_days — numeric representation of purchase frequency


Exported the cleaned dataset for SQL and Power BI use

2. 📊 Exploratory Data Analysis (Python)

Plotted histograms and box plots for numerical distributions
Used bar charts and count plots for categorical breakdowns (gender, category, segment)
Generated a correlation heatmap to identify feature relationships
Visualised segment distributions across age groups, seasons, and shipping preferences

3. 🗄️ SQL Analysis (MySQL)
Loaded the cleaned dataset into a MySQL table and authored 10 business queries:
#Business Question1Total revenue by gender2Discount users spending above average3Top 5 products by average review rating4Avg. spend — Express vs. Standard shipping5Subscriber vs. non-subscriber spend comparison6Top 5 products by discount usage rate7Customer segmentation — New / Returning / Loyal (CTE)8Top 3 products per category (Window Function: ROW_NUMBER)9Repeat buyers (>5 purchases) and subscription status10Revenue contribution by age group
4. 📈 Power BI Dashboard

Imported cleaned dataset and built a relational data model
Created KPI cards, bar charts, donut charts, and trend lines
Enabled dynamic filtering by gender, category, season, subscription status, and age group
(See Dashboard section below)

5. 📝 Project Report

Compiled findings, methodology, SQL results, and recommendations into a structured Word/PDF report
Covers data pipeline, key insights, and business recommendations

6. 🎨 Presentation (Gamma)

Built a clean, visual slide deck using Gamma
Summarises the problem, approach, key findings, and recommendations for a non-technical audience


📊 Dashboard
The Power BI dashboard features 4 interactive report pages with cross-filtering across all visuals:
PageContentOverviewKPI cards — Total Revenue, Avg. Purchase, Total Customers, Subscriber RateDemographicsGender split, age group breakdown, location distributionProduct & CategoryBest-selling categories, top-rated products, discount usageCustomer BehaviourPurchase frequency, shipping preference, payment method, loyalty segments
Slicers available: Gender · Category · Season · Subscription Status · Age Group

🔍 Key Results

68% male customer base — female segment is underrepresented and presents a growth opportunity
Subscribers (27%) show higher average spend and stronger revenue contribution per head
Middle-aged adults drive the highest revenue across all age groups
Customers who applied discounts still exceeded average spend — confirming a high-value deal-seeker segment
Repeat buyers (>5 purchases) show a strong propensity for subscriptions — a ready-made conversion cohort
Top-rated products are concentrated in specific sub-categories — ideal for featured placement in marketing


📁 Project Structure
customer-behaviour-analytics/
│
├── data/
│   ├── customer_raw.csv               # Original dataset
│   └── customer_cleaned.csv           # Cleaned & transformed dataset
│
├── notebooks/
│   └── eda_cleaning.ipynb             # Python EDA & cleaning notebook
│
├── sql/
│   └── business_queries.sql           # 10 SQL business queries
│
├── dashboard/
│   └── Customer_Behaviour_Dashboard.pbix   # Power BI dashboard file
│
├── report/
│   └── Customer_Behaviour_Project_Report.pdf
│
├── presentation/
│   └── Customer_Behaviour_Slides.pdf  # Exported Gamma slide deck
│
└── README.md

👤 Author
Shubham
https://www.linkedin.com/in/shubham-kumar-b54382267/
