\# Zuber Ride-Sharing SQL Analysis

\#\# Project Description  
This project was conducted as part of an analysis for \*\*Zuber\*\*, a ride-sharing company launching in Chicago. The goal was to identify patterns in passenger preferences and assess the impact of external factors, such as weather conditions, on ride frequency and duration. By analyzing a comprehensive dataset, we aimed to provide insights to optimize the company's operations and improve customer experience.

\#\# Data Description  
The dataset consists of several tables containing information on taxi rides in Chicago:

\- \*\*neighborhoods\*\*: Data on the neighborhoods in the city.  
  \- \`neighborhood\_id\`: Unique identifier for each neighborhood.  
  \- \`name\`: Name of the neighborhood.

\- \*\*cabs\*\*: Data on taxi vehicles and their respective companies.  
  \- \`cab\_id\`: Unique identifier for each cab.  
  \- \`vehicle\_id\`: Technical ID of the vehicle.  
  \- \`company\_name\`: The name of the taxi company.

\- \*\*trips\*\*: Data on individual taxi rides.  
  \- \`trip\_id\`: Unique identifier for each ride.  
  \- \`cab\_id\`: Reference to the vehicle that provided the ride.  
  \- \`start\_ts\`: Timestamp of when the ride started.  
  \- \`end\_ts\`: Timestamp of when the ride ended.  
  \- \`duration\_seconds\`: Duration of the ride in seconds.  
  \- \`distance\_miles\`: Distance of the ride in miles.  
  \- \`pickup\_location\_id\`: Neighborhood code where the ride started.  
  \- \`dropoff\_location\_id\`: Neighborhood code where the ride ended.

\- \*\*weather\_records\*\*: Data on weather conditions during the rides.  
  \- \`record\_id\`: Unique identifier for each weather record.  
  \- \`ts\`: Timestamp when the weather data was recorded.  
  \- \`temperature\`: Temperature at the time of the record.  
  \- \`description\`: Brief description of weather conditions (e.g., 'light rain').

\#\# Problems Solved  
The analysis aimed to address several key questions about Zuber's ride-sharing operations:  
\- \*\*Ride frequency by company\*\*: We analyzed the number of rides provided by each taxi company over a specific period.  
\- \*\*Impact of weather on ride duration\*\*: We explored how weather conditions, especially rain, affected the duration of trips between key locations.  
\- \*\*Passenger preferences\*\*: By grouping rides based on companies and neighborhoods, we aimed to identify patterns in customer behavior and preferred services.

\#\# Key Tasks and Methodology  
1\. \*\*Exploratory Data Analysis (EDA)\*\*:  
   \- Task 1: Counted the number of rides for each taxi company between November 15–16, 2017\. The results were grouped by company and sorted by the number of rides in descending order.  
   \- Task 2: Filtered the data for taxi companies whose names contain "Yellow" or "Blue" for rides between November 1–7, 2017\.  
   \- Task 3: Analyzed ride data for two of the most popular taxi companies, \*\*Flash Cab\*\* and \*\*Taxi Affiliation Services\*\*, during November 1–7, 2017\. Other companies were grouped into a category called "Other."

2\. \*\*Weather Impact Analysis\*\*:  
   \- Task 4: Retrieved the neighborhood identifiers for the \*\*Loop\*\* and \*\*O'Hare\*\* neighborhoods to assess trips between these two points.  
   \- Task 5: Created a new weather conditions field (\`weather\_conditions\`) using the \`CASE\` statement to categorize the weather as either "Good" or "Bad" based on the presence of rain or storm in the description.  
   \- Task 6: Joined weather data with trip data to analyze how weather conditions affected trip durations on Saturdays for trips starting in the Loop and ending at O'Hare.

\#\# Findings  
\- \*\*Ride Frequency by Company\*\*: The company with the highest number of rides between November 15–16, 2017, was identified. By filtering for companies like \*\*Yellow\*\* and \*\*Blue\*\*, we narrowed down the most active companies during the November 1–7, 2017, period.  
\- \*\*Weather’s Impact on Ride Duration\*\*: Rides from the Loop to O'Hare on rainy Saturdays took longer than rides on clear days, showing a clear correlation between adverse weather and increased ride durations.  
\- \*\*Passenger Preferences\*\*: Flash Cab and Taxi Affiliation Services were the most popular companies, while other companies had significantly fewer rides.

\#\# Tools and Technical Skills  
\- \*\*SQL\*\*: Used for querying and analyzing the dataset.  
\- \*\*JOINs\*\*: Leveraged to combine data from multiple tables, such as trips and weather records.  
\- \*\*CASE Statements\*\*: Utilized to create new fields based on conditional logic, such as categorizing weather conditions.  
\- \*\*Grouping and Aggregation\*\*: Used to count rides by company and analyze ride frequencies over time.

\#\# View My Project  
You can view the screenshots and the SQL queries used for the project \[here\](link-to-your-screenshots-or-repo).