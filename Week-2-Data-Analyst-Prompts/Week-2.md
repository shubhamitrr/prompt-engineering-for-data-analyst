***# Week 2 — Data Analyst Prompts***



***## 1. Excel Prompts***



***An Excel prompt is a clear instruction given to AI to help with Excel formulas, data cleaning, analysis, formatting, and other Excel tasks.***



***### Example***



***> I have student marks in cell A2. Write an Excel formula to show "Pass" if marks are 40 or above, otherwise "Fail".***



***```excel***

***=IF(A2>=40,"Pass","Fail")***

***```***



***### Uses***



***\* IF, SUMIF, COUNTIF***

***\* XLOOKUP/VLOOKUP***

***\* Data cleaning***

***\* Date calculations***

***\* Pivot Tables***

***\* Excel analysis***



***### Key Takeaway***



***Give AI the \*\*cell/column information + task + expected result\*\*.***



***---***



***## 2. SQL Prompts***



***A SQL prompt is a clear instruction given to AI to create, explain, debug, or improve SQL queries.***



***### Example***



***> Write a MySQL query to find the top 5 employees with the highest salary from the employees table.***



***```sql***

***SELECT name, salary***

***FROM employees***

***ORDER BY salary DESC***

***LIMIT 5;***

***```***



***### Uses***



***\* Query generation***

***\* JOIN***

***\* GROUP BY***

***\* HAVING***

***\* Window Functions***

***\* CTE***

***\* Subqueries***

***\* SQL error fixing***

***\* Query optimization***



***### Key Takeaway***



***Mention the \*\*database, table, columns, and exact task\*\*.***



***---***



***## 3. Python/Pandas Prompts***



***A Python/Pandas prompt is a clear instruction to AI to write, explain, debug, or improve Python/Pandas code.***



***### Example***



***> Write Python Pandas code to find the top 5 rows with the highest Sales from DataFrame df.***



***```python***

***df.nlargest(5, "Sales")***

***```***



***### Another Example***



***```python***

***df.groupby("Region")\["Sales"].sum()***

***```***



***This calculates total Sales for each Region.***



***### Uses***



***\* Data cleaning***

***\* Missing values***

***\* Duplicates***

***\* Filtering***

***\* GroupBy***

***\* Sorting***

***\* EDA***

***\* Debugging***



***### Key Takeaway***



***Tell AI \*\*what DataFrame you have + what operation you need\*\*.***



***---***



***## 4. Data Cleaning Prompts***



***A data cleaning prompt asks AI to identify and fix problems in a dataset.***



***Common problems:***



***\* Missing values***

***\* Duplicate rows***

***\* Wrong data types***

***\* Spelling inconsistencies***

***\* Extra spaces***

***\* Invalid values***

***\* Outliers***



***### Example***



***> You are a Data Analyst. Analyze DataFrame df for missing values and duplicate rows. Show their counts and provide Pandas code to handle them.***



***### Example***



***Replace missing Age values with the median:***



***```python***

***df\["Age"] = df\["Age"].fillna(df\["Age"].median())***

***```***



***### Key Takeaway***



***\*\*Problem → Cleaning Method → Code → Check Result\*\****



***---***



***## 5. EDA Prompts***



***EDA means \*\*Exploratory Data Analysis\*\*.***



***An EDA prompt asks AI to explore a dataset and identify patterns, distributions, relationships, and important findings.***



***### Example***



***> You are a Data Analyst. Perform EDA on the provided sales dataset. Check dataset structure, missing values, duplicate rows, numerical summary, sales distribution, and the relationship between Sales and Profit. Provide key findings in bullet points.***



***### Useful Pandas functions***



***```python***

***df.shape***

***df.info()***

***df.isnull().sum()***

***df.duplicated().sum()***

***df.describe()***

***```***



***### EDA Flow***



***\*\*Load Data → Clean Data → Explore Data → Find Patterns → Generate Insights\*\****



***---***



***## 6. Visualization Prompts***



***A visualization prompt tells AI which chart to create or recommend for a dataset.***



***### Example***



***> You are a Data Analyst. I have monthly sales data from January to December. Create a line chart to show the sales trend over time using Python Matplotlib.***



***### Common Charts***



***| Chart        | Purpose                   |***

***| ------------ | ------------------------- |***

***| Bar Chart    | Compare categories        |***

***| Line Chart   | Show trends over time     |***

***| Scatter Plot | Show relationships        |***

***| Histogram    | Show distribution         |***

***| Box Plot     | Distribution and outliers |***



***### Key Takeaway***



***A good visualization prompt contains:***



***\*\*Data + Purpose + Chart Type + Tool + Expected Output\*\****



***---***



***## 7. Statistical Analysis Prompts***



***A statistical analysis prompt asks AI to calculate and explain statistical measures.***



***### Common Measures***



***\* Mean → Average***

***\* Median → Middle value***

***\* Mode → Most frequent value***

***\* Standard Deviation → Spread of data***

***\* Correlation → Relationship between variables***



***### Example***



***> You are a Data Analyst. Calculate the mean, median, minimum, maximum, and standard deviation of the Sales column. Explain each result in simple English.***



***### Pandas Example***



***```python***

***df\["Sales"].mean()***

***df\["Sales"].median()***

***df\["Sales"].std()***

***```***



***### Key Takeaway***



***Ask AI for both \*\*calculation and interpretation\*\* when needed.***



***---***



***## 8. Business Insight Prompts***



***A business insight prompt asks AI to analyze data and identify findings that are useful for understanding business performance.***



***### Example***



***> You are a Data Analyst. Analyze the sales data and identify the top-performing and low-performing regions. Explain the possible business insights in simple bullet points.***



***### Important Difference***



***\*\*Analysis:\*\****

***Region A has the highest sales.***



***\*\*Insight:\*\****

***Region A is performing better than other regions.***



***\*\*Recommendation:\*\****

***Investigate what factors are driving Region A's performance.***



***Keep these three separate.***



***### Key Takeaway***



***A Data Analyst should convert \*\*numbers → findings → business meaning\*\*.***



***---***



***## 9. Power BI Prompts***



***A Power BI prompt is a clear instruction to AI for Power BI tasks such as Power Query, data modeling, visuals, dashboards, and analysis.***



***### Example***



***> You are a Power BI expert. I have a sales dataset with Product, Category, Region, Sales and Profit columns. Suggest suitable Power BI visuals for a sales dashboard and explain what each visual should show.***



***### Uses***



***\* Power Query***

***\* Data cleaning***

***\* Data modeling***

***\* Relationships***

***\* Dashboard design***

***\* Visual selection***

***\* Filters and slicers***

***\* DAX***

***\* Business insights***



***### Dashboard Example***



***\* KPI → Total Sales and Profit***

***\* Bar Chart → Sales by Category***

***\* Map → Sales by Region***

***\* Line Chart → Monthly Sales***



***### Key Takeaway***



***\*\*Dataset + Columns + Power BI Task + Expected Output\*\****



***---***



***## 10. DAX Prompts***



***A DAX prompt is a clear instruction given to AI to create, explain, fix, or improve DAX formulas in Power BI.***



***### Example***



***> Write a DAX measure to calculate total sales from the Sales column in the Sales table.***



***```DAX***

***Total Sales = SUM(Sales\[Sales])***

***```***



***### Profit Margin Example***



***```DAX***

***Profit Margin =***

***DIVIDE(***

&#x20;   ***SUM(Sales\[Profit]),***

&#x20;   ***SUM(Sales\[Sales])***

***)***

***```***



***### Uses***



***\* SUM***

***\* AVERAGE***

***\* COUNT***

***\* CALCULATE***

***\* IF***

***\* SWITCH***

***\* Percentage calculations***

***\* Profit Margin***

***\* Year-over-Year analysis***

***\* Running totals***

***\* Measures***

***\* DAX error fixing***



***### Key Takeaway***



***Tell AI the \*\*table + columns + required calculation + expected output\*\*.***



***---***



***# Week 2 Summary***



***Data Analyst prompts help AI with different parts of the Data Analyst workflow:***



***\*\*Excel → SQL → Python/Pandas → Data Cleaning → EDA → Visualization → Statistics → Business Insights → Power BI → DAX\*\****



***### Good Data Analyst Prompt Formula***



***\*\*Role + Context + Task + Constraints + Output Format\*\****



***The more specific and clear the prompt is, the more useful the AI response can be.***



