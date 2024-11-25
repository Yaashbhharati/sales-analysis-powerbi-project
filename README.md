
# Sales Analysis Dashboard

---

## Problem Statement  

The **Sales Analysis Dashboard** is designed to help organizations make data-driven decisions by analyzing sales trends, identifying performance metrics, and discovering improvement areas.  

This dashboard provides:  
- Insights into overall sales and profitability.  
- Identification of top-performing products, regions, and time periods.  
- Key metrics to assess revenue growth and operational efficiency.  

By understanding these patterns and trends, businesses can enhance their strategies, allocate resources effectively, and boost overall profitability.  

---

## Steps Followed  

1. **Data Loading**:  
   - Data was loaded into Power BI Desktop from CSV/Excel files.  

2. **Data Cleaning**:  
   - Power Query Editor was used to profile, clean, and transform the dataset:  
     - Checked **Column Quality**, **Column Distribution**, and **Column Profile**.  
     - Filtered out null or irrelevant data (e.g., blank sales records).  
     - Ensured appropriate data types for all fields.  

3. **Data Transformation**:  
   - Created calculated columns using Power Query (M Code).  
   - Removed duplicates and ensured a clean dataset.  

4. **Data Modeling**:  
   - Established relationships between sales, customers, and product tables.  
   - Defined star schema for easier analysis.  

5. **Visualizations**:  
   - Added slicers for key filters like **Region**, **Product Category**, and **Time Period**.  
   - Designed visuals such as:  
     - Line charts for time-based sales trends.  
     - Pie charts for regional distribution.  
     - Bar charts for product-wise performance.  

6. **DAX Measures**:  
   - Defined custom measures for:  
     - Total Sales  
     - Profit Margin  
     - Year-over-Year (YoY) Growth  
     - Average Revenue per Customer  

7. **Dashboard Design**:  
   - Used themes for consistent styling.  
   - Incorporated company branding, including logo and color palette.  

8. **Publishing**:  
   - Published the report to Power BI Service for access and collaboration.  

---

## Key Features  

1. **Sales Trends**:  
   - Visualize monthly, quarterly, and yearly sales trends.  

2. **Profitability Insights**:  
   - Track profit margins and contribution by product and region.  

3. **Customer Analysis**:  
   - Breakdown of sales by customer segments (e.g., age group, purchase frequency).  

4. **KPIs**:  
   - Key Performance Indicators showing total sales, profit, and growth rate.  

5. **Interactivity**:  
   - Dynamic slicers and filters for deeper analysis.  

---

## Insights  

### Overall Sales Performance  
- **Total Sales**: $118.73M  
- **Profit **: 16.89M 
- **Top-Performing Region**: USA 

### Trends and Patterns  
- Revenue peaks during [specific time periods, e.g., Q4].  
- Decline observed in sales for [underperforming products/regions].  


---

## DAX Calculations  

Examples of DAX measures used in the dashboard:  

- **Total Sales**:  
  ```DAX  
  Total Sales = SUM(Sales[Amount])  
  ```  

- **Profit Margin**:  
  ```DAX  
  Profit Margin = DIVIDE(SUM(Sales[Profit]), SUM(Sales[Amount]))  
  ```  

- **YoY Growth**:  
  ```DAX  
  YoY Growth =  
      DIVIDE(  
          [Total Sales] - CALCULATE([Total Sales], DATEADD(Calendar[Date], -1, YEAR)),  
          CALCULATE([Total Sales], DATEADD(Calendar[Date], -1, YEAR))  
      )  
  ```  

---

## Steps to Access  

1. **Clone the Repository**:  
   ```bash  
   git clone https://github.com/yourusername/sales-analysis-dashboard.git  
   ```  

2. **Open the Dashboard**:  
   - Download and open the `.pbix` file in Power BI Desktop.  

3. **View the Report**:  
   - If using Power BI Service, access the published report via the link provided.  

4. **Explore**:  
   - Use slicers and filters to view custom insights.  

---

## Future Enhancements  

- Automate data updates using real-time data pipelines.  
- Integrate predictive analytics for sales forecasting.  
- Expand customer segmentation analysis.  

---

---

## Contact  

For questions or feedback:  

- **Name**:YASH BHARATI
- **Email**: yashbharati8@gmail.com
- **GitHub**: https://github.com/Yaashbhharati
---
