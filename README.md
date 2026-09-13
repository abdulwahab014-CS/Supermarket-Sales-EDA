# Supermarket-Sales-EDA

## Project Description
This is an Exploratory Data Analysis (EDA) project evaluating a 1,000-transaction supermarket dataset across three branch locations to uncover pricing dynamics, category performance metrics, and customer engagement drivers using Python, Pandas, Matplotlib, and Seaborn.

## Dataset Description
The dataset has 1,000 rows and 17 columns covering retail store transaction records, customer demographics, financial metrics, and store satisfaction ratings.

## Technologies Used
* **Languages & Libraries**: Python, Pandas, NumPy, Matplotlib & Seaborn
* **Environment**: Google Colab Notebook

## Analysis Performed
1. **Data Cleaning Process**
2. **Feature Analysis**
3. **Correlation Analysis**
4. **12+ Visualizations**

## Key Findings
* **Low-to-mid price concentration**: 75% of product unit prices are under $77.94, the median unit price is $55.23, and the mean is $55.67.
* **Category volume**: Fashion accessories and Food & beverages lead: Fashion accessories with 178 transactions and Food & beverages with 174 transactions are the largest categories by order volume.
* **Revenue leader**: Food & beverages generated the highest total revenue at $56,144.84 across 174 transactions, closely followed by Sports & travel at $55,122.83.
* **Price and rating aren't correlated**: Unit price and customer rating have almost no correlation (r = -0.009). Higher prices do not yield higher customer ratings.
* **Quantity drives revenue**: Purchase quantity shows a strong positive correlation with overall order revenue (r = 0.71), proving that multi-unit order volume drives revenue more effectively than unit price (r = 0.63).
* **Rating vs. transaction spend**: Rating and total spend have a near-zero correlation (r = -0.036). Customer satisfaction operates independently of basket size.
* **Price outliers**: Using the IQR method, 9 transactions are high-value spend outliers exceeding $991.74, reaching up to $1,042.65 for 10-unit bulk purchases.
* **Ratings are solid overall**: The average customer satisfaction rating across the store is 6.97 out of 10.0 stars.
* **Smallest revenue category**: Health & beauty recorded the lowest total revenue at $49,193.74, representing a $6,951.10 deficit relative to Food & beverages.
* **Branch leader**: Branch C in Naypyitaw led all supermarket locations with $110,568.71 in total revenue.
* **Member vs. Non-Member spend**: Registered Members spent $327.79 per basket on average, slightly outspending Normal non-members at $318.12.
* **Gender spend gap**: Female shoppers generated higher overall revenue ($167,882.93) and spent $24.31 more per transaction on average than male shoppers.
* **Male dominance in Health & Beauty**: Male customers generated $30,632.75 in Health & Beauty sales compared to $18,560.99 from female shoppers (65% higher male spend).
* **Payment channel preferences**: Cash led overall store spending ($112,206.57), closely followed by E-wallets ($109,993.11).
* **Peak shopping hours**: Transaction volume peaks sharply at 13:00 ($34,723.23) and 19:00 ($39,699.51), dropping off significantly by 20:00.

## 5 Business Recommendations
1. **Target male consumers in Health & Beauty**: Male shoppers spent 65% more in Health & Beauty than female shoppers ($30,632.75 vs $18,560.99). Expanding male personal care inventory will lift this lowest-performing category ($49,193.74 total).
2. **Launch mid-week 'Monday Boost' promos**: Monday generated the lowest revenue of the week at $37,899.08 (32.4% below Saturday's peak of $56,120.81). Mid-week promotional discounts will help balance weekly customer traffic.
3. **Incentivize multi-unit bundling**: Correlation analysis shows purchase quantity (r = 0.71) drives top-line revenue more than unit price (r = 0.63). Offering multi-buy promotional bundles (e.g., "Buy 2 Get 1 Discounted") will increase average basket size above 5.51 units.
4. **Transition to dynamic margin tiers**: The supermarket currently applies a flat 4.76% gross profit margin across all inventory lines. Transitioning to dynamic 8–12% margins on high-demand categories like Food & Beverages and Fashion Accessories will expand gross income.
5. **Optimize peak hour checkout staffing**: Reallocate cashier shift schedules to cover peak shopping hours (13:00 and 19:00) to minimize checkout wait times, while offering evening E-wallet discounts to boost late-hour sales.

## Step-by-Step Guide to Run the Project

1. **Download the Dataset**: Locate the `supermarket_sales.csv` file in this repository. Click on the file and click Download to save a copy of it to your local computer.
2. **Open the Notebook in Google Colab**: Go to Google Colab. Click on File > Upload notebook. Choose or drag-and-drop the `code.ipynb` file from this repository.
3. **Upload the Dataset to Colab**: Once the notebook is open in Google Colab, look at the left-hand sidebar and click on the Folder (Files) icon. Click the Upload button (an icon of a file with an upward arrow) and upload your downloaded `supermarket_sales.csv` file into the `/content/` directory so the pandas file-reading path works properly.
4. **Run the Analysis**: Click on Runtime in the top menu bar. Select Run all to execute all data cleaning, statistical analysis, and visualization cells sequentially from top to bottom.
