Marketing Campaign Analysis
Analyzed FreshChoice Foods' marketing campaign data to identify customer segments with the highest campaign acceptance rates and provide actionable targeting recommendations.

Data
Source: Client brief (Client_Brief_FreshChoice_Foods.docx) containing customer demographics, purchase history, and campaign response data
Size: 2,240 customers, 29 features
Cleanup: Handled nulls, fixed data types, normalized income brackets, split marital status and education into clean categorical fields
Process
Cleaned raw data — addressed missing values, standardized formats
Loaded into SQLite — split into 4 relational tables for querying
Exploratory SQL queries — 7 business questions answered with aggregation, filtering, and window functions
Segmentation analysis — compared acceptance rates across income, education, family status, country, and product spend segments
Report — compiled findings into a Word document (FreshChoice_Campaign_Analysis_Report.docx)
Key Findings
Segment	Acceptance Rate
Overall baseline	14.9%
High-income (>80k)	40.0%
No kids/teens	26.5%
High-income + no kids	41.5%
PhD holders	20.8%
Basic education	3.7%
Top insight: Customers earning >80k with no children accepted Campaign 6 at 41.5% — nearly 3x the baseline. This 188-person segment alone generated 78 acceptances.

Tools
Python (pandas) — data cleaning and normalization
SQLite — relational database with 4 tables, 7 analytical queries using CTEs and window functions
python-docx — report generation
Files
File	Description
Marketing_Campaign_Analysis.ipynb	Full notebook with code, outputs, and insights
freshchoice.db	SQLite database with cleaned data
FreshChoice_Campaign_Analysis_Report.docx	Final report
marketing_data.csv	Raw input data
Client_Brief_FreshChoice_Foods.docx	Original client brief
Recommendation
Focus Campaign 6 on high-income customers without children — highest ROI segment at 41.5% acceptance vs 14.9% baseline.
