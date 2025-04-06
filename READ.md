A) My Approach
1) Load Olist dataset CSVs using Pandas.
2) Use SQLAlchemy to write data into SQL Server.

B) KPI Calculation:

Write a Python script (compute_customer_kpis()) to compute:

Total unique customers
Number of customers per state
Most common customer city

C) Storage:

Save each KPI result into a separate table in SQL Server.

D) Visualization:

In Jupyter Notebook, read the KPI tables and generate:

Text summaries
A bar chart for customers by state.




Prompts I Used for the LLM
SQLAlchemy
matplotlib/seaborn chart for KPIs from SQL Server



What I Had to Figure Out Myself

Used schema="dbo" explicitly to avoid table visibility issues



KPI Choices and Business Relevance

Total Unique Customers	Number of distinct customers                       
Customers by State	Distribution of customers across Brazil	           
Most Common City	City with the highest number of customers	   



 Challenges Faced
Used raw strings (e.g., r"C:\path") to avoid Unicode errors
to_sql() table not appearing then Added schema="dbo"


