#  BigBasket Product Data Analysis

##  Problem Statement
BigBasket is facing challenges in ensuring timely deliveries, especially during peak hours and in high-demand regions. These issues impact customer satisfaction, increase operational costs, and reduce resource efficiency. This project aims to **optimize delivery operations** and **enhance the customer experience** using data analytics.

---

##  Project Goal

To **leverage data analytics** to:
- Enhance operational efficiency
- Improve customer satisfaction
- Drive sustainable growth through data-driven decision-making

---

##  Dataset Description

The dataset consists of **27,555 rows** and **10 columns**, each representing different product attributes:

| Column        | Description                                |
|---------------|--------------------------------------------|
| `index`       | Row number                                  |
| `product`     | Product name                                |
| `category`    | Product's main category                     |
| `sub_category`| More specific classification                |
| `brand`       | Product's brand name                        |
| `sale_price`  | Current sale price                          |
| `market_price`| Original market price                       |
| `type`        | Type of product                             |
| `rating`      | Customer rating                             |
| `description` | Product description                         |

---

##  Technologies Used

- Python (Pandas, NumPy)
- Data Visualization: Matplotlib, Seaborn, Plotly
- Jupyter Notebook

---

##  EDA Steps

###  Step 1: Load and Inspect Data
- Read CSV file
- Display first 12 rows
- Check info & summary statistics

###  Step 2: Handle Missing Values
- Ratings and descriptions had missing values
- Imputed missing fields with `"Unknown"`

###  Step 3: Outlier Detection & Treatment
- Used IQR method
- Applied to `sale_price`, `market_price`, and `rating`

###  Step 4: Discount Analysis
- Calculated discount as a percentage
- Identified high-discount items

###  Step 5: Identify Top/Least Sold Products
- Based on frequency of product names

---

##  Visualizations & Insights

###  Histogram Distributions
- **Ratings**: Mostly between 4.0 - 4.5
- **Market Prices**: Highly skewed; spike around ₹800
- **Sale Prices**: Majority under ₹200; spike at ₹700

###  Pie Chart: Product Sub-Categories
- **Skin Care**: 16.1%
- **Health & Medicine**: 7.9%
- Other categories: Hair Care, Snacks, Spices, etc.

###  Brand Rating Analysis
- **Highest Rated Brands**: "1mg", "6 Rasa"
- Ratings gradually decline across brands

###  Density & Violin Plots
- Sale and market prices show right-skewed distributions
- Rating distribution is bimodal
- Violin plots highlight price variation and density

###  Scatter Plot
- Sale Price vs Rating: No strong linear correlation, but visible clusters

###  Bar Plots
- Top 15 brands by product count
- Top 5 products by rating

---

##  Key Insights

- Majority of products are priced under ₹200, indicating affordability
- "Skin Care" leads in product variety
- A few brands dominate in quality (high ratings)
- Data cleaning significantly improved dataset reliability

---

##  Recommendations

- Focus marketing on highly-rated and high-frequency items
- Investigate underperforming brands or categories
- Leverage peak sale price ranges for promotions

---

##  Conclusion

This EDA provided actionable insights for BigBasket’s inventory, pricing, and customer preferences. These findings can support **logistics optimization**, **customer satisfaction strategies**, and **data-driven growth**.

---

##  Project Structure

```bash
bigbasket-project/
│
├── BigBasket_Analysis.ipynb     # Jupyter notebook with full analysis
├── BigBasket_Products.csv       # Raw dataset
├── README.md                    # Project documentation
└── images/                      # Visualizations and charts (optional)

 Author

Shane Alam  
Aspiring Data Analyst | Python & EDA Enthusiast  
 India  
 Email: [alamshane2043@gmail.com]  
 LinkedIn: [https://www.linkedin.com/in/shane-alam-36317a2a7/]
