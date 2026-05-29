
# Customer Shopping Behavior Analysis

# 📊 Project Overview
This project analyzes customer shopping behavior using transactional data from 3,900 purchases across various product categories. The primary objective is to uncover actionable insights into spending patterns, customer segments, product preferences, and subscription behavior to help guide strategic business decisions.

#  📂 Dataset Summary 

* Total Records: 3,900 rows

* Features: 18 columns

* Key Data Points:

  *  **Customer Demographics:** Age, Gender, Location, Subscription Status

  * **Purchase Details:** Item Purchased, Category, Purchase Amount, Season, Size, Color

  * **Shopping Behavior:** Discount Applied, Promo Code Used, Previous Purchases, Frequency of Purchases, Review Rating, Shipping Type

* Note: Handled 37 missing values in the Review Rating column during the data cleaning phase.

 # 🛠️ Tools & Technologies Used
 * **Python (Pandas):** Data Loading, Cleaning, Feature Engineering, and Exploratory Data Analysis (EDA).

* **PostgreSQL (SQL):** Advanced querying to extract business metrics and transaction trends.

* **Power BI:** Building an interactive dashboard for visual data storytelling.
 # 🚀 Project Workflow

   **1. Data Cleaning & EDA (Python)**

* **Exploration:** Analyzed dataset structure and summary statistics using pandas.

* **Imputation:** Filled missing Review Rating values using the median rating of each respective product category.

* **Standardization:** Converted all column headers to snake_case for seamless SQL integration.

* **Feature Engineering:** - Created an age_group column by binning customer ages.

  * Calculated a purchase_frequency_days metric from purchase history.

* **Validation:** Resolved redundancies between discount_applied and promo_code_used.

**2. Business Insights & Analysis (SQL)**

Loaded the cleaned dataset into PostgreSQL to answer key business questions:

* **Revenue by Gender:** Male customers generated higher total revenue ($157,890) compared to female customers ($75,191).

* **Product Performance:** Identified the top 5 highest-rated products (Gloves, Sandals, Boots, Hat, Skirt) and the top 3 sellers per category.

* **Subscription Impact:** Compared spending habits between subscribers (27% of users) and non-subscribers (73%).

* **Discount Dependencies:** Pinpointed the top 5 products most frequently bought with a discount (Hats led at 50%).

* **Customer Segmentation:** Grouped the customer base into Loyal (3,116), Returning (701), and New (83) segments.

**3. Data Visualization (Power BI)**

Built an interactive Customer Behavior Dashboard highlighting:

* Top-level KPIs: 3.9K Customers, $59.76 Avg. Purchase, 3.75 Avg. Rating.

* Revenue and Sales distributions split by Age Group and Product Category.

* Demographic compositions (Gender, Subscription Status) and Shipping Type preferences.

 # Business Recommendations

Based on the analysis, the following strategic actions are recommended:

  - **Boost Subscriptions:** Introduce exclusive perks and targeted promotions to increase the current 27% subscriber base.

- **Launch Loyalty Programs:** Incentivize repeat buyers to transition more "Returning" customers into the highly valuable "Loyal" segment.

- **Review Discount Policies:** Re-evaluate discount dependencies on specific items (like Hats and Sneakers) to balance sales volume with profit margin control.

- **Optimize Product Positioning:** Feature top-rated and consistently best-selling products prominently in marketing campaigns.

- **Implement Targeted Marketing:** Focus ad spend and campaigns on the highest revenue-driving age groups (Young Adults and Middle-aged) and users who prefer express shipping.
