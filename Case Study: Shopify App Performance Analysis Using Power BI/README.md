# Case Study: Shopify App Landscape and Reviews Analysis with PowerBI

## Project Overview

The primary goal of this project is to analyze the landscape of apps in the Shopify marketplace, identifying key factors contributing to app success. Using data scraped from publicly available Shopify websites, we focus on understanding the correlation between various app metrics and their success in the market, with a detailed examination of app reviews, ratings, and developer responsiveness.

The project consists of three parts:

1. **App Landscape Overview** - To understand the general structure of the Shopify app ecosystem.
2. **App Reviews Analysis** - A deeper dive into app reviews, including metrics on developer responsiveness and helpfulness of reviews.
3. **Developer Analysis** - Evaluating developer behavior and success factors based on their app’s performance and user feedback.

## Tools & Techniques Used

- **Power BI Desktop** for visualization and data modeling.
- **DAX (Data Analysis Expressions)** for creating calculated columns.
- **Scatterplots, Line Charts, and Bar Charts** to display relationships and trends across key app metrics.
- **Advanced Filtering and Relationships** between multiple datasets.
- **KPI Cards** for high-level summary metrics.

## Part 1: App Landscape

### KPI Card: Total Number of Apps
- **Visualization**: The first visual is a simple KPI Card that displays the total number of unique apps in the dataset.
- **Finding**: The Shopify marketplace contains **7,341** apps, which represents the extent of available solutions to Shopify users.

![KPI Card](https://github.com/albertohg1/Data_projects_TripleTen/blob/297ddc4377e31b60ad25f1431824fda99df36dc8/Case%20Study%3A%20Shopify%20App%20Performance%20Analysis%20Using%20Power%20BI/Sprint%206%20PowerBI%201.1.png)

### Line Chart: Sum of Review Counts Over Time
- **Visualization**: A line chart visualizing the sum of review counts for apps over time, based on their last modified date (`lastmod`).
- **Finding**: A sharp peak in the review count occurs early in May, followed by a consistent but lower level of reviews.

![Line Chart](https://github.com/albertohg1/Data_projects_TripleTen/blob/297ddc4377e31b60ad25f1431824fda99df36dc8/Case%20Study%3A%20Shopify%20App%20Performance%20Analysis%20Using%20Power%20BI/Sprint%206%20PowerBI%201.2.png)

### Scatterplot: Number of Reviews vs Average Rating
- **Visualization**: A scatterplot showing the correlation between the number of reviews and the average rating.
- **Finding**: Apps with high numbers of reviews tend to maintain high ratings, but there is significant variance for apps with fewer reviews. Some highly reviewed apps have lower ratings, suggesting possible issues with scaling user satisfaction.

![Scatterplot](https://github.com/albertohg1/Data_projects_TripleTen/blob/297ddc4377e31b60ad25f1431824fda99df36dc8/Case%20Study%3A%20Shopify%20App%20Performance%20Analysis%20Using%20Power%20BI/Sprint%206%20PowerBI%201.3.png)

## Part 2: App Reviews

### New Column: Helpful Reviews
- **DAX Formula**: `helpful_reviews = rating * (1 + helpful_count)`.
- **Card Visualization**: The average value of helpful reviews is calculated and displayed using a KPI Card. 
- **Finding**: The average weighted value of helpful reviews is **5.48**, indicating that many reviews provide useful feedback that influences overall ratings.

![Helpful Reviews](https://github.com/albertohg1/Data_projects_TripleTen/blob/297ddc4377e31b60ad25f1431824fda99df36dc8/Case%20Study%3A%20Shopify%20App%20Performance%20Analysis%20Using%20Power%20BI/Sprint%206%20PowerBI%202.1.png)

### Scatterplot: Developer Answered vs Average Rating
- **Visualization**: A scatterplot comparing the average rating based on whether a developer answered the review.
- **Finding**: There is a positive correlation between developer responsiveness and higher average ratings. Apps where developers responded to reviews typically have higher ratings, reinforcing the importance of customer support and engagement.

![Scatterplot](https://github.com/albertohg1/Data_projects_TripleTen/blob/297ddc4377e31b60ad25f1431824fda99df36dc8/Case%20Study%3A%20Shopify%20App%20Performance%20Analysis%20Using%20Power%20BI/Sprint%206%20PowerBI%202.2.png)

## Part 3: Developer Analysis

### Bar Chart: Developer vs Sum of Ratings
- **Visualization**: A bar chart showing the sum of ratings for each developer. 
- **Finding**: Certain developers like **Elfsight** and **Omega** have amassed the highest total ratings, likely due to the volume of apps and user interactions.

![Sum of Ratings by Developer](https://github.com/albertohg1/Data_projects_TripleTen/blob/297ddc4377e31b60ad25f1431824fda99df36dc8/Case%20Study%3A%20Shopify%20App%20Performance%20Analysis%20Using%20Power%20BI/Sprint%206%20PowerBI%203.1.png)

### Bar Chart: Developer vs Average of Helpful Reviews
- **Visualization**: A bar chart showing the average helpful review scores by developer.
- **Finding**: Developers like **Picorem** and **GreenPod** have the highest average helpful review scores, indicating that their apps provide significant value and users appreciate their contributions to the marketplace.

![Average Helpful Reviews by Developer](https://github.com/albertohg1/Data_projects_TripleTen/blob/297ddc4377e31b60ad25f1431824fda99df36dc8/Case%20Study%3A%20Shopify%20App%20Performance%20Analysis%20Using%20Power%20BI/Sprint%206%20PowerBI%203.2.png)

### Bar Chart: Developer Responsiveness
- **Visualization**: A bar chart showing the number of times a developer answered user reviews, filtered to only show apps with more than 500 reviews.
- **Finding**: **FireApps** and **Dosers** lead in responsiveness, with over 6,000 instances where developers have answered user queries. Developer engagement seems to be a strong predictor of app success and customer satisfaction.

![Developer Responsiveness](https://github.com/albertohg1/Data_projects_TripleTen/blob/297ddc4377e31b60ad25f1431824fda99df36dc8/Case%20Study%3A%20Shopify%20App%20Performance%20Analysis%20Using%20Power%20BI/Sprint%206%20PowerBI%203.3.png)

## Conclusion

This Power BI project provided a comprehensive analysis of the Shopify app landscape, with a particular focus on understanding user feedback and developer responsiveness. Key insights include:

- High numbers of reviews correlate with higher app ratings, but outliers exist.
- Developer responsiveness significantly influences average app ratings.
- Certain developers lead the market in terms of both helpful reviews and engagement with users.

By focusing on these factors, developers can improve their apps’ success and increase customer satisfaction. This analysis also provides critical insights for Shopify to enhance its app store’s value to users by highlighting app quality and developer engagement.

