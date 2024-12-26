### **Project Background**  
XYZ Corp, a mid-sized retail company specializing in online and brick-and-mortar sales. The management team is focused on understanding sales trends, customer behavior, and operational performance to optimize decision-making
processes. 

**Insights and recommendations** are provided on the following key areas:
- **Sales & Profit Trends Analysis**: Evaluation of historical sales patterns, by region, focusing on Revenue, Profit, and Order Volume.
- **Product Level Performance**: An analysis of JohnMart’s various product lines, understanding their impact on sales and returns.
- **Regional Comparisons**: An evaluation of sales and orders by region.

An interactive Tableau dashboard can be viewed: [here](https://public.tableau.com/app/profile/tariq.ijaz/viz/SalesDashboard_17331991909900/SalesDashboard)

---

### **Data Structure & Initial Checks**  
XYZ Corp’s data structure consists of **3 tables**: **Sales_data**, **Operational_data**, **Customer_data**, with **1000 records** excluding headers. We have a total of **3 years of data from 2023-2025**.  

![Data Structure](https://github.com/user-attachments/assets/eb7b95ee-8612-451e-80c3-7683dec18f4f)


Data Completeness: The Sales_data and Operational_data sheets contains complete data with no missing values.
Data Integrity: There are no duplicate Order IDs in the dataset.
Key Integration Challenge: The main data quality issue is the absence of Customer ID in the Sales_n_Operational_Combined sheet, which prevents us from joining it with the customer_data sheet. This limitation impacts our ability to perform detailed customer segmentation analysis and calculate customer-specific metrics.

Impact on Analysis:

We can accurately analyze sales trends, product performance, and operational metrics
We cannot perform customer-specific analyses such as customer lifetime value or customer segmentation
Regional and product analyses remain reliable as they don't depend on customer data

---

### **Executive Summary**  

#### **Overview of Findings**  
- **Sales Revenue** increased by around **50%** from **2021-2023**. The growth has been steady year-over-year:
  - **2021 to 2022**: Revenue increased by **29.5%**, ending with total sales of **$609K**.
  - **2022 to 2023**: Revenue increased by **20.4%**, ending with total sales of **$733K**.

- **Total Profit** increased by around **50%** from **2021-2023**, with a slowing growth rate:
  - **2021 to 2022**: Profit increased by **24.7%**, ending with total profit of **$82K**.
  - **2022 to 2023**: Profit increased by **12.5%**, ending with total profit of **$93K**.

- **Order Volume** increased by around **55%** from **2021-2023**:
  - **2021 to 2022**: Orders increased by **26.7%**.
  - **2022 to 2023**: Orders increased by **28.3%**.
  - **Key Insight**: Volume continues to be a major driver of sales.

- **Total Customers** increased by around **27.1%** from **2021-2023**:
  - **2021 to 2022**: Customers increased by **16.3%**.
  - **2022 to 2023**: Customers increased by **10.8%**.

---

### **Sales Trends**  
The company’s sales showed consistent year-over-year growth from **2021 to 2023**, with notable seasonal peaks in December.  

- **2021**: Sales began with moderate performance but improved significantly by year-end.  
- **2022**: Sales peaked in **December** at **$609K**, reflecting a **29.5% increase** compared to 2021. The post-holiday dip in **January 2022** was followed by stable growth throughout the year.  
- **2023**: Sales continued to grow, reaching **$733K** in December, representing a **20.4% year-over-year increase**.  
- **Key Insights**: While overall growth remained positive, the rate of revenue growth moderated in 2023. Q4 consistently performed the strongest, highlighting reliance on seasonal demand.  

---

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
