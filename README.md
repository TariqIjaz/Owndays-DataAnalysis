# **Project Background**  
XYZ Corp is a mid-sized retail company specializing in online and brick-and-mortar sales. The management team is focused on understanding sales trends, customer behavior, and operational performance to optimize decision-making
processes. 

**Insights and recommendations** are provided on the following key areas:
- **Sales & Profit Trends Analysis**: Evaluation of historical sales patterns by region, focusing on Revenue, Profit, and Order Volume.
- **Product Level Performance**: An analysis of XYZ Corp’s various product lines, understanding their impact on sales and returns.
- **Regional Comparisons**: An evaluation of sales and orders by region.

An interactive Tableau dashboard can be viewed: <br><a href="https://public.tableau.com/app/profile/tariq.ijaz/viz/OwndaysSalesDashboard/OverviewDash?publish=yes" target="_blank">here</a>

---
# **Data Structure & Initial Checks**

XYZ Corp’s data structure consists of **3 tables**: **Sales_data**, **Operational_data**, and **Customer_data**, containing a total of **1000 records** (excluding headers). The dataset spans **3 years (2023–2025)**.

![image](https://github.com/user-attachments/assets/d690dbee-e2d3-4e89-90b5-2e308d5ca500)
---

### **Data Completeness**
1. All three sheets contain complete data with no missing values.
2. The data for the year **2025 ends in September**, preventing a full 3-year sales trend analysis. Missing data from **October to December 2025** creates an artificial dip in sales.

### **Data Integrity**
- No duplicate **Order IDs** were identified in the dataset, ensuring data reliability.

### **Key Integration Challenge**
- The **Sales_data** sheet lacks a **Customer ID** column, making it impossible to join with the **Customer_data** sheet.
- This limitation affects our ability to:
  - Perform **customer segmentation**.
  - Calculate **customer-specific metrics** (e.g., customer lifetime value).

---

# **Executive Summary**

## **Key Findings**

### **Overall Sales and Profit Trends**
- **Sales** peaked at **$250.9K** in 2024 (+4.3% YoY) but dropped significantly to **$210.2K** in 2025 (-16.2% YoY), partly due to missing data from October–December 2025.
- **Profit** mirrored sales trends, increasing from **$19.5K** in 2023 to **$20.5K** in 2024 (+5%) before declining sharply to **$15.6K** in 2025 (-24% YoY).
- **Profit margins** were stable between 2023 and 2024 (8.1% to 8.2%) but fell to **7.4%** in 2025, indicating cost pressures or pricing challenges.

**Overall 2023 - 2024**
![image](https://github.com/user-attachments/assets/72788df1-cbe8-4872-a7bd-71d07d1641f4)

-
**Overall 2024 - 2025**
![image](https://github.com/user-attachments/assets/0eccb040-9374-405e-9cff-36cb550fccd7)


### **Customer and Order Metrics**
- **Customer numbers** were stagnant at **200** across all years, highlighting a lack of growth in customer acquisition.
- **Order volume** increased slightly from **365** in 2023 to **366** in 2024 before falling to **269** in 2025 (-26.5%), reflecting lower customer demand.
- **Average Order Value (AOV)** increased over the three years: **$141.6** in 2023, **$145.0** in 2024, and **$166.3** in 2025. Despite fewer orders in 2025, the higher AOV suggests larger transactions per order

### **Regional Insights**
- **Region 2** consistently outperformed others in sales and profit through 2024 but faced the steepest decline in 2025 (-17.6% sales, -25% profit).
- **Regions 3 and 4** consistently lagged, with high shipping costs and delivery delays contributing to lower performance.
- **Region 1** demonstrated efficient logistics and relatively smaller declines (-16.4% sales, -24.2% profit).

| Regional Sales (2023 - 2024) | Regional Sales (2024-2025) |
|:---:|:---:|
| ![image](https://github.com/user-attachments/assets/024313f4-a235-4746-9f53-a10aa624a127) | ![image](https://github.com/user-attachments/assets/75108c25-92be-42a7-aed0-8558c268f158) |

-
| Regional Profit (2023 - 2024) | Regional Profit (2024 - 2025) |
|:---:|:---:|
| ![Regional Profit 2023-2024](https://github.com/user-attachments/assets/359b5513-0355-4189-be9c-da1fa34ad630) | ![Regional Profit 2024-2025](https://github.com/user-attachments/assets/8bdf3604-50c2-4a6d-be5c-2bf94026449b) |


### **Category, Subcategory, and Product Performance**
- **Category 3** exhibited the highest growth in 2024 (+6%) but saw the sharpest decline in 2025 (-17.3%), reflecting demand volatility.
- **Subcategory 5** and top products (e.g., **49**, **50**, **40**) consistently ranked as high performers in both sales and profit.
- Profitability dropped across all **categories** and **subcategories** in 2025 due to increased costs or reduced demand.

| Category Sales (2023 - 2024) | Category Sales (2024-2025) |
|:---:|:---:|
| ![image](https://github.com/user-attachments/assets/d18c544f-0c3a-4a80-934b-0b4f400d59bb) | ![image](https://github.com/user-attachments/assets/74fe53e5-c016-4db0-80c7-ae5486ee4022) |
-
| Category Profit (2023 - 2024) | Category Profit (2024 - 2025) |
|:---:|:---:|
| ![image](https://github.com/user-attachments/assets/4a3c7e02-08d1-4791-ad43-71d31ed2f9af) | ![image](https://github.com/user-attachments/assets/86cf994e-21da-4ac3-a49c-68e61e267c34) |


### **Demographics**
- Customers were evenly split between **males** and **females**, with the most active age group being **26–65**, consistent across all years.

---

## **Recommendations**

### **Customer Acquisition**
- **Launch targeted marketing campaigns** aimed at increasing the customer base, focusing on the **26–65 age group**. (Due to missing customer_ID in the sales_data sheet, we have limited drill-down capabilities)
- Introduce **loyalty programs** or **incentives** to convert occasional buyers into repeat customers.

### **Operational Efficiency**
- **Region 3 and 4 Logistics**: Implement cost-reduction strategies and streamline delivery processes to reduce shipping costs and delays.
- **Benchmark with Region 1**: Use Region 1’s operational model as a template to improve logistics across other regions.

### **Data Integrity and Missing Records**
- Ensure **complete and accurate data collection** to prevent gaps like the missing October–December 2025 data.
- Standardize **data validation processes** to maintain analysis reliability.

### **Product and Pricing Strategy**
- Leverage **high-performing subcategories** and products like **Subcategory 5** and products **49, 50, 40** by expanding their availability and promoting them further.
- Conduct a **cost-benefit analysis** to reassess pricing strategies and reduce cost pressures impacting profit margins.
- Leverage the increasing AOV by analyzing which **products or services** contribute most to this growth and expanding these offerings.

### **Market Analysis and Strategy**
- Conduct a **root cause analysis** to identify factors behind the significant decline in 2025 sales and profits, focusing on external market dynamics (e.g., competition, economic conditions) and internal inefficiencies (missing data (October - December 2025).
- **Reignite growth in Region 2** through new product launches and strategic partnerships.

### **Risk Mitigation for Volatility**
- Develop **contingency plans** to prepare for market downturns, such as diversifying product lines or identifying alternative revenue streams to mitigate losses.

---

## **Next Steps**
1. Assign a **dedicated team** to address the operational inefficiencies in Regions 3 and 4, focusing on cost and delivery optimizations.
2. Conduct a **workshop** to redesign the 2025 marketing strategy, leveraging insights from 2023–2024 trends.
3. Perform a **detailed profitability analysis** of underperforming products and categories to identify areas for improvement.
4. Implement a **robust data management system** to ensure complete and accurate reporting for all future analyses.

---
## **Assumptions and Caveats**

Throughout the analysis, multiple assumptions were made to manage challenges with the data. These assumptions and caveats are noted below:

1. **Product Categorization**:
   - All products (e.g., Product 1 to Product 50) are assigned to multiple categories (e.g., Product 1 belongs to all of Categories 1, 2, and 3).
   - Since there is no documentation about the business type or what the products represent in the case study document, the **subcategory analysis** provides a better categorical breakdown as the products are uniquely categorized under the subcategory.

2. **Profit Calculation**:
   - The documentation does not explicitly state whether the **shipping cost** is already factored into the profit column in the `Sales_data` tab. Additionally, there is no indication of whether the profit represents **Gross** or **Net Profit**.
   - It is assumed that **shipping costs** and **OPEX** have been factored in, and the column represents **Net Profit**.

3. **Customer Data Limitations**:
   - The `customer_data` tab includes columns such as Customer ID, Name, Age, Gender, Email, and Region. However, the `sales_data` tab lacks a **Customer ID** or similar column to directly relate sales to customers in the `customer_data`.
   - Joining solely on **Region** would create a many-to-many relationship, which is not logically valid because multiple customers can belong to the same region, and the `sales_data` does not specify which customer made each purchase.
   - As a result, in-depth analyses such as **customer purchasing behavior**, **customer lifetime value**, and **sales/profit by demographics** are limited due to these constraints.

4. **Shipping Cost Application**:
   - It is assumed that the **shipping cost** is applied to a **total order** rather than individual item quantities.

5. **Sales Amount and Discounts**:
   - The `sales_amount` column does not explicitly state if the amount is **before or after the discount**.
   - For the analysis, it is assumed that the sales amount represents the **pre-discount** value, while the sales amounts shown in charts are calculated **after discounts**.

----
# **Detailed Analysis** 

## **Overview of Findings**

### **Trends**

#### **Sales Growth**
- Sales increased from **$240.4K** in 2023 to **$250.9K** in 2024, showing a 4.3% growth year-over-year (YoY).
- In 2025, sales dropped significantly to **$210.2K**, reflecting a decline of 16.2% compared to 2024. Missing records from October onwards might have contributed to this drop.

#### **Profit and Profit Margin**
- Profit improved from **$19.5K** in 2023 to **$20.5K** in 2024, showing a 5% YoY increase.
- However, profit declined sharply to **$15.6K** in 2025, a 24% decrease compared to 2024.
- Profit margins remained relatively stable between 2023 and 2024 (8.1% to 8.2%) but fell to **7.4%** in 2025, indicating possible cost increases or pricing issues.

#### **Orders**
- The number of orders showed a slight increase from **365** in 2023 to **366** in 2024 (+0.3%).
- In 2025, orders dropped significantly to **269**, a 26.5% decrease compared to the previous year. This decline aligns with the drop in sales and could reflect lower customer demand or operational challenges.

#### **Customer Retention**
- The total number of customers remained consistent at **200** across all three years, indicating no net customer growth.

#### **Average Order Value (AOV)**
- AOV steadily increased over the three years: **$141.6** in 2023, **$145.0** in 2024, and **$166.3** in 2025.
- Despite fewer orders in 2025, the higher AOV suggests larger transactions per order, possibly due to a focus on premium products or price adjustments.

---

### **Insights**
- The consistent number of customers with no growth highlights a need for **customer acquisition strategies**.
- The increase in AOV is a positive trend, but the decline in orders and sales in 2025 suggests operational challenges or external factors affecting demand.
- Profit margin reduction in 2025 indicates a potential **cost management issue** or an imbalance in the pricing strategy.
- The sharp drop in metrics for 2025 (October onwards) could be attributed to **missing records**, emphasizing the importance of complete and accurate data for analysis.

---

## **Region Performance**

### **Sales Trends by Region**

#### **Region 1**
- 2023: **$64.59K**
- 2024: **$66.68K** (+3.2%)
- 2025: **$55.72K** (-16.4%)
- After slight growth in 2024, sales in Region 1 declined significantly by 16.4% in 2025, indicating challenges such as reduced demand or operational inefficiencies.

#### **Region 2**
- 2023: **$69.12K**
- 2024: **$73.39K** (+6.2%)
- 2025: **$60.44K** (-17.6%)
- Region 2 showed strong growth in 2024 but faced the steepest decline among all regions in 2025, possibly due to external market challenges or competition.

#### **Region 3**
- 2023: **$51.88K**
- 2024: **$54.01K** (+4.1%)
- 2025: **$45.71K** (-15.4%)
- Sales in Region 3 fell by 15.4% in 2025, reversing the moderate growth seen in previous years.

#### **Region 4**
- 2023: **$54.82K**
- 2024: **$56.78K** (+3.6%)
- 2025: **$48.35K** (-14.8%)
- Region 4 experienced consistent growth in 2024, followed by a notable drop in 2025.

---

### **Profit Trends by Region**

#### **Region 1**
- 2023: **$4.40K**
- 2024: **$4.58K** (+4.1%)
- 2025: **$3.47K** (-24.2%)

#### **Region 2**
- 2023: **$5.26K**
- 2024: **$5.59K** (+6.3%)
- 2025: **$4.20K** (-25.0%)

#### **Region 3**
- 2023: **$4.46K**
- 2024: **$4.67K** (+4.8%)
- 2025: **$3.57K** (-23.5%)

#### **Region 4**
- 2023: **$5.39K**
- 2024: **$5.63K** (+4.5%)
- 2025: **$4.33K** (-23.2%)

---

### **Shipping Cost vs. Delivery Days by Region**
- **Region 1**: Lowest average shipping cost and delivery days, maintaining operational efficiency across all years.
- **Region 2**: Balanced shipping costs and delivery times, maintaining reliability.
- **Regions 3 and 4**: Highest shipping costs and delivery times, possibly contributing to declining sales and profits in 2025.

---

## **Category, Subcategory, and Product Performance**

### **Sales Trends by Categories**
- **Category 1**: Peaked in 2024 ($84.06K) before declining to $70.12K in 2025 (-16.6% YoY).
- **Category 2**: Similar trends, falling to $70.30K in 2025 (-14.7% YoY).
- **Category 3**: Highest growth in 2024 (+6%) but steepest decline in 2025 (-17.3%).

### **Top-Performing Subcategories**
1. **Subcategory 5**: Most profitable subcategory across all years.
2. **Subcategory 4**: Strong but declined in 2025.

### **Top Products**
- Products **49**, **50**, and **40** consistently delivered the highest sales and profits.

### **Demographics**
- Customers were evenly split between genders, with the 26–65 age group accounting for the majority of purchases.

