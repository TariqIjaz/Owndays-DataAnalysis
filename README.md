### **Project Background**  
XYZ Corp is a mid-sized retail company specializing in online and brick-and-mortar sales. The management team is focused on understanding sales trends, customer behavior, and operational performance to optimize decision-making
processes. 

**Insights and recommendations** are provided on the following key areas:
- **Sales & Profit Trends Analysis**: Evaluation of historical sales patterns by region, focusing on Revenue, Profit, and Order Volume.
- **Product Level Performance**: An analysis of XYZ Corp’s various product lines, understanding their impact on sales and returns.
- **Regional Comparisons**: An evaluation of sales and orders by region.

An interactive Tableau dashboard can be viewed:<br><a href="https://public.tableau.com/app/profile/tariq.ijaz/viz/OwndaysSalesDashboard/OverviewDash?publish=yes" target="_blank">here</a>

---

### **Data Structure & Initial Checks**  
XYZ Corp’s data structure consists of **3 tables**: **Sales_data**, **Operational_data**, **Customer_data**, with **1000 records** excluding headers. We have **3 years of data from 2023-2025**.  

![image](https://github.com/user-attachments/assets/d690dbee-e2d3-4e89-90b5-2e308d5ca500)

Data Completeness: 
1)The Sales_data and Operational_data sheets contain complete data with no missing values.
2) The data for the year 2025 ends in September. This will prevents us from getting a full complete 3 year sales trends, as we would anticipate a dip in sales due to  missing months (November & December)
Data Integrity: There are no duplicate Order IDs in the dataset.
Key Integration Challenge: The main data quality issue is the absence of Customer ID in the Sales_data sheet, which prevents us from joining it with the customer_data sheet. This limitation impacts our ability to analyze detailed customer segmentation and calculate customer-specific metrics.

Impact on Analysis:
We can accurately analyze sales trends, product performance, and operational metrics
We cannot perform customer-specific analyses such as customer lifetime value or customer segmentation
Regional and product analyses remain reliable as they don't depend on customer data

---

## **Executive Summary**  

### **Overview of Findings**

Over the three-year period, the company experienced fluctuating sales, profits, and operational metrics, highlighting areas of success and emerging challenges.

Key Performance Trends:
Sales:

2023: Total sales stood at $43.9K, with strong performance in June and December, indicating seasonal trends.
2024: Sales grew slightly to $45.1K (+2.6% YoY) due to a strong start in January and consistent peaks mid-year.
2025: Sales declined sharply to $38.0K (-15.8% YoY) due to reduced orders and missing data for October onwards.
Profit:

2023: Total profit was $3.5K, maintaining a modest margin.
2024: Profit rose slightly to $3.6K (+3.7% YoY) despite modest sales growth, indicating improved cost efficiency.
2025: Profit fell to $2.8K (-23.7% YoY) as a result of declining sales and increased operational challenges.
Orders and Customers:

Orders decreased significantly from 365 in 2023 to 269 in 2025 (-26.5% YoY from 2024 to 2025), reflecting a worrying trend of reduced purchase activity.
Customer count remained stagnant at 200 across all three years, highlighting a lack of growth in customer acquisition.
Seasonality:

Peak sales months remained consistent (June, August, and December) across years, underscoring opportunities to leverage seasonal trends.
Early months like January 2024 performed well, contrasting with weaker starts in 2023 and 2025.
Key Insights:
Growth Plateau: After modest growth in 2024, the business faced a substantial downturn in 2025, likely driven by reduced order volumes and stagnant customer acquisition.
Profit Margin Challenges: The declining profit in 2025 suggests cost inefficiencies or a drop in pricing power, which needs immediate attention.
Customer Retention Issues: The lack of growth in the customer base, despite some sales improvements, indicates potential gaps in customer engagement or acquisition strategies.
Recommendations:
Boost Customer Acquisition:

Implement targeted marketing campaigns and loyalty programs to attract and retain customers.
Address any barriers to entry for new customers, such as pricing or user experience.
Improve Operational Efficiency:

Optimize cost structures to prevent profit erosion.
Analyze product margins and eliminate low-margin offerings where necessary.
Leverage Seasonal Trends:

Double down on successful months (June, August, December) with tailored campaigns and inventory planning.
Explore promotions during historically weaker months to drive off-season sales.
Enhance Data Completeness:

Ensure consistent and accurate data collection across all months to enable a comprehensive year-over-year analysis and better decision-making.
Conclusion:
While 2024 showed some progress, the significant drop in sales and profit in 2025 signals the need for immediate strategic action. Focusing on customer acquisition, cost management, and leveraging seasonal opportunities will be critical to reversing the current downward trend and achieving sustainable growth.



---
### Region Performance

Regional Performance Summary (2023–2025):

Region 1 (Texas):

Sales:
2023: $12.94K
2024: $13.02K (+0.6% vs. 2023)
2025: $11.04K (-15.2% vs. 2024)

Profit:
2023: $874
2024: $892 (+2.0% vs. 2023)
2025: $684 (-23.3% vs. 2024)

Key Insights:
Region 1 remains the leader in sales and profit but experienced sharp declines in both metrics in 2025.
Despite modest growth in 2024, the region saw a significant erosion of profitability in 2025.

Region 2 :

Sales:
2023: $11.54K
2024: $11.99K (+3.9% vs. 2023)
2025: $9.99K (-16.7% vs. 2024)

Profit:
2023: $872
2024: $912 (+4.6% vs. 2023)
2025: $691 (-24.3% vs. 2024)

Key Insights:
Region 2 saw the strongest profit growth in 2024 (+4.6%) but suffered the steepest declines in both sales and profit in 2025.
The decline indicates inefficiencies or weakened customer demand.
Region 3:

Sales:
2023: $10.33K
2024: $10.73K (+3.9% vs. 2023)
2025: $8.94K (-16.7% vs. 2024)

Profit:
2023: $881
2024: $922 (+4.6% vs. 2023)
2025: $697 (-24.3% vs. 2024)

Key Insights:
Region 3 followed a similar trajectory to Region 2, with consistent profit growth in 2024 but a steep decline in 2025.
Underperformance in 2025 signals operational or market-related challenges.
Region 4:

Sales:
2023: $9.10K
2024: $9.33K (+2.5% vs. 2023)
2025: $7.99K (-14.3% vs. 2024)

Profit:
2023: $890
2024: $923 (+3.6% vs. 2023)
2025: $712 (-22.8% vs. 2024)

Key Insights:
Region 4 had the smallest decline in sales in 2025 but still experienced significant profit loss (-22.8%), highlighting inefficiencies in cost management.
Trends and Observations:
2023:
Sales and profit showed steady performance, with Region 4 achieving the highest profit despite being the lowest in sales.
2024:
All regions experienced sales and profit growth, with Regions 2 and 3 leading in profit increases (+4.6%).
Investments in operational efficiency likely drove profit growth, even in lower-performing regions like Region 4.
2025:
A sharp downturn occurred across all regions, with profit declines exceeding sales drops in percentage terms.
Regions 2 and 3 saw the steepest losses (-24.3%) in profit, while Region 4 was comparatively less affected.

Opportunities and Recommendations:
Focus on Cost Management:

The disproportionate decline in profits in 2025 suggests rising costs or inefficient pricing strategies. Implement cost-cutting measures and refine pricing models across all regions.
Revitalize Underperforming Regions:

Target Regions 2 and 3 with specific initiatives to recover both sales and profitability. This includes customer engagement strategies, discounts, and operational optimizations.
Sustain Growth in Region 4:

Despite being the lowest in sales, Region 4 demonstrated relative profit resilience. Leverage this trend to further stabilize and grow this region.
Capitalize on Peak Seasons:

Across all years, profits and sales consistently peaked mid-year (May–July). Expand marketing and inventory strategies during these months to maximize returns.
Conduct Root-Cause Analysis:

Investigate the drivers behind the widespread declines in 2025. Consider factors such as economic conditions, customer behavior, or operational inefficiencies.




### **Product Performance**  

- **Top-Performing Categories**:  
  - **Furniture** and **Technology** drove the largest share of revenue, with subcategories like **Phones**, **Chairs**, and **Copiers** showing consistent profitability.  
  - **Accessories** emerged as a growing segment, contributing significantly to both order volume and profit.  

- **Underperforming Subcategories**:  
  - **Tables** and **Bookcases** showed recurring losses. These products had lower profit margins and were impacted by high discounting.  
  - **Labels** and **Supplies** also contributed minimally to overall revenue and exhibited low performance.  

- **High-Performing Products**:  
  - Specific product lines, such as high-end **Chairs** and **Phones**, dominated revenue contributions and profitability.  

---

### **Recommendations**  

1. **Diversify Product Offerings**:  
   - With growing success in **Accessories**, expand product lines for Samsung and Apple ecosystems, such as premium cables and wireless chargers, to capitalize on upsell opportunities.  

2. **Address Underperforming Products**:  
   - Evaluate the viability of **Tables** and **Bookcases**. Discontinue or bundle slow-moving products to improve profitability.  
   - Implement promotional strategies such as flash sales or bundled pricing to clear low-performing inventory like **Labels** and **Supplies**.  

3. **Enhance Seasonal Strategies**:  
   - Q4 remains the strongest period; launch targeted marketing campaigns earlier in Q3 to capture pre-holiday demand and boost year-end performance.  

4. **Increase Focus on High-Profit Subcategories**:  
   - Prioritize marketing and inventory optimization for **Phones**, **Chairs**, and **Copiers**, as they drive significant revenue and margins.  

5. **Leverage Data for Personalization**:  
   - Use customer purchase history to drive personalized marketing, particularly for products with repeat purchase potential (e.g., **Accessories** and office supplies).  

By focusing on product diversification, improving inventory performance, and optimizing seasonal marketing strategies, the company can sustain long-term growth while addressing areas of underperformance.


### **Assumptions and Caveats**:

Throughout the analysis, multiple assumptions were made to manage challenges with the data. These assumptions and caveats are noted below:

1) All products (e.g., Product 1 to Product 50) are assigned to multiple categories (e.g., Product 1 belongs to all of Categories 1, 2, and 3). Since there is no documentation about the business type or what the products represent in the case study document, the subcategory analysis will provide a better picture for a categorical breakdown as the products are uniquely categorized under the sub-category. 


2) The documentation does not explicitly mention that the shipping cost is already factored in the profit column in the Sales_data tab. In addition, there is no indication of Gross or Net Profit. I will assume that the shipping cost and OPEX have been factored in, and that column is the Net Profit.


3) The customer_data has columns like Customer ID, Name, Age, Gender, Email, and Region. However, the sales_data does not have a Customer ID or similar column to relate it to the customers in customer_data directly. Joining only on Region would create a many-to-many relationship, which is not logically valid because multiple customers can belong to the same region, and the sales_data does not specify which customer made each purchase. Conducting an in depth customer purchasing analysis, customer lifetime value and sales/profit by demographics are limited due to this limiting condition. 


4) I also assume that the shipping cost is applied to a total order rather than to the item quantity.


5) The sales amount does not state if the amount is before or after the discount. I will assume that it is before the discount. The sales amount shown on the charts are  sales after discount.



