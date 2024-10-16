\# Case Study: Strategic Insights into Superstore Returns: A Tableau Dashboard Analysis

\#\# Project Overview  
In this project, I developed a comprehensive analysis for the CEO of Superstore to help them understand what is causing customers to return their orders. The goal was to find insights into why returns happen and how they can be minimized. The project included building a Tableau dashboard and storytelling component to visualize the findings and communicate actionable insights effectively.

\#\# Problem Statement  
The main issue facing the Superstore was a high volume of returned orders. Through this analysis, I sought to identify:  
\- Key drivers behind returns  
\- Correlations between returns and various factors such as product category, customer behavior, and geographic distribution  
\- Potential seasonal patterns impacting return rates

\#\# Dataset Used  
The dataset consisted of two tables:  
1\. \*\*Orders Table\*\*: Containing data about customer orders, including product, region, customer ID, sales, and profits.  
2\. \*\*Returns Table\*\*: Containing information about whether each order was returned (Yes/No).

The two tables were joined using a \*\*LEFT JOIN\*\*, ensuring that we could track both returned and non-returned orders.

\#\# Analytical Approach  
\#\#\# 1\. Data Cleaning:  
\- A calculated field was created to convert null values in the "Returned" column to 0 and "Yes" values to 1, allowing us to compute return rates.  
\- Filtered out customers with only one order to focus on frequent customers with a pattern of returns.

\#\#\# 2\. Visual Analysis:  
Several key visualizations were built to analyze the return rates from different perspectives:

\- \*\*Scatter Plot \- Sales vs. Returns\*\*: Demonstrates whether high sales correlate with high returns across product subcategories.  
\- \*\*Bar Chart \- Return Rate by Category\*\*: Visualizes the return rates by product category (Furniture, Technology, Office Supplies).  
\- \*\*Bar Chart \- Return Rate by Customer\*\*: Highlights the customers with the highest return rates, allowing the store to identify customer behavior.  
\- \*\*Map \- Return Rate by State\*\*: Geographically displays return rates, identifying states where returns are more prevalent.  
\- \*\*Line Graph \- Return Rate by Month\*\*: Analyzes return rates by month to detect any seasonal patterns.  
\- \*\*Combined Line and Bar Chart \- Sales vs. Return Rate by Month\*\*: Shows the trend of sales alongside return rates over time.  
\- \*\*Lollipop Chart \- Profits vs Return Rate by Region\*\*: Combines profits and return rates by region to assess performance from both perspectives.

\#\# Findings and Insights  
1\. \*\*High Return Rate in Specific Categories\*\*: Technology products had the highest return rate (27.3%), followed by Office Supplies and Furniture, which indicates that the store might need to focus on product quality or set better customer expectations in these categories.  
     
2\. \*\*Geographic Insights\*\*: The map revealed that certain regions, particularly the West and East, had significantly higher return rates compared to other areas.

3\. \*\*Seasonal Trends\*\*: The analysis indicated higher return rates in September and March, suggesting potential seasonal effects on returns.

4\. \*\*Customer Behavior\*\*: Some customers consistently had a 100% return rate, which points to a pattern that might need special attention (e.g., targeted communication or incentive programs to reduce returns).

5\. \*\*Sales vs. Returns Correlation\*\*: The scatter plot of sales vs returns showed that higher sales didn’t necessarily mean higher returns, suggesting that other factors besides volume were contributing to returns.

\#\# Technical Skills Used  
\- \*\*Tableau\*\*: For creating data visualizations, dashboards, and a Tableau Story for presenting findings.  
\- \*\*Data Cleaning\*\*: Using calculated fields and joins to clean and prepare data for analysis.  
\- \*\*Statistical Analysis\*\*: Identifying trends, patterns, and correlations in data using advanced Tableau features like dual-axis charts and combined graphs.

\#\# Tableau Links  
\- \*\*Tableau Dashboard\*\*: \[Link to Dashboard\](https://public.tableau.com/views/Sprint5StorytellingwithDataProject-JoseAlbertoHernandez/ReturnRateAnalysis?:language=en-US\&publish=yes&:sid=&:redirect=auth&:display\_count=n&:origin=viz\_share\_link)  
\- \*\*Tableau Story\*\*: \[Link to Tableau Story\](https://public.tableau.com/views/Sprint5StorytellingwithDataProject-JoseAlbertoHernandez/SuperstoreReturnRateAnalysis2?:language=en-US\&publish=yes&:sid=&:redirect=auth&:display\_count=n&:origin=viz\_share\_link)  
\- \*\*Video Presentation\*\*: \[Link to Video Presentation\](https://drive.google.com/file/d/1-0GpFbgr9PZ3vmY2bcvyxmKP42r\_hl0F/view?usp=sharing)

\---

This project helped the Superstore CEO gain insights into the causes of returns and identify potential strategies for reducing them, thus improving profitability and customer satisfaction.

