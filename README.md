# DataMagnet:Transforming Real Estate Data into Actionable Insights

It involves of a structured database to store and manage information related to Airbnb listings, hosts, reviews, and other relevant data. The primary goal is to perform analysis and gain insights from this data for various purposes.
              
 # What is this system all about?
The system as a whole seems to model the backend structure of an application where users can list properties, make bookings, leave reviews, and where hosts manage their listings. The SQL queries provide the means to create, populate, and query this database structure.

The provided set of SQL queries represents a database schema and operations related to managing data for a fictional online rental platform, presumably similar to Airbnb. 

The tables are Listings, Hosts, Availability, and Reviews. They are designed to store information about property listings, hosts, availability dates, and reviews, respectively. 
![image](https://github.com/ishanimahajan20/ANALYSIS-OF-AIRBNB-DATA-USING-SQL/assets/134215344/97fff9b4-f682-4aaf-8f17-567eb79bebab)

# Why we need this system?
A system like this one describe how SQL queries is typically designed for managing data in an online rental platform, similar to Airbnb. 

We created this for following reasons :
1. Data Organization -> Organization is essential for efficient data storage, retrieval, and management.
2. User Interaction -> For users of the platform (hosts, guests, and administrators), the system facilitates interaction with the data. Hosts can manage their property listings, guests can search for and book accommodations, and administrators can oversee the platform's operations.
3. Search and Retrival -> Database structure supports complex queries that enable users to search for specific listings, filter results based on criteria like availability or price, and retrieve relevant information about hosts and reviews.
4. Booking and Reservation Handling -> The inclusion of a Booking table suggests that the system can handle the booking process, including details such as check-in and check-out dates.
5. Review and rating System -> This feature allows guests to provide feedback on their stay, helping future guests make informed decisions.

# What is the scope of this system?
The system's scope is broad, covering aspects from user interaction to backend data management. Its utility lies in creating a seamless and secure environment for users and hosts to engage in rental transactions while providing the platform administrators with the tools to oversee and optimize the overall operation.

# In this project, I have demonstrated :

1. Designing a robust relational database schema.
-> Define tables, relationships, and constraints to organize data efficiently.

2. Implementing complex SQL queries for searching and filtering listings.
-> Use SELECT statements with WHERE clauses to filter data based on specified criteria.

3. Optimizing queries for performance.
-> Utilize indexes, avoid unnecessary JOINs, and optimize complex queries for faster execution.

4. Managing user and property data efficiently.
-> Use INSERT, UPDATE, and DELETE statements to handle user and property data modifications.

5. Handling transactions and ensuring data consistency.
-> Use transactions (BEGIN TRANSACTION, COMMIT, ROLLBACK) to ensure data consistency during complex operations.

6. Designing database triggers for automatic updates.
-> Create triggers to automatically perform actions (INSERT, UPDATE, DELETE) based on specified conditions.

7. Employing joins, subqueries, and aggregations effectively.
-> Use INNER/OUTER JOINs, subqueries, and aggregate functions (e.g., SUM, AVG) for complex data retrieval.

8. Ensuring data security and privacy through appropriate access controls.
-> Implement GRANT and REVOKE statements to control user access to specific database objects.

9. Adhering to best practices in database normalization and indexing.
-> Organize data to minimize redundancy and use indexes for efficient data retrieval.

10. Demonstrating problem-solving skills in addressing specific project requirements.
-> Create SQL queries that address specific challenges posed by the project requirements.

# Who are the key stakeholders in this system?
Key stakeholders include hosts, administrators, reviewers, data analysts, marketing, IT support, and product development teams. They collectively contribute to the platform's success and functionality.

# WHAT ARE WE TRYING TO EVALUATE?
We are trying to evaluate the performance, user satisfaction, and efficiency of the Airbnb-like platform.
This involves assessing factors like booking rates, customer reviews, host satisfaction, system uptime, revenue generation, and user feedback. The evaluation aims to understand how well the platform meets its goals and identifies areas for improvement.

![image](https://github.com/ishanimahajan20/ANALYSIS-OF-AIRBNB-DATA-USING-SQL/assets/134215344/43f69b8f-07a5-4daf-8cf8-62211eddeb3b)
![image](https://github.com/ishanimahajan20/ANALYSIS-OF-AIRBNB-DATA-USING-SQL/assets/134215344/99809786-5948-49df-818c-aa5052ccf15a)
![image](https://github.com/ishanimahajan20/ANALYSIS-OF-AIRBNB-DATA-USING-SQL/assets/134215344/dd656968-c06b-45f0-9686-b4c1cea6ede9)

# ER DIAGRAM:

-> A Property is owned by an Owner.
-> A Transaction involves a Property, Buyer, and Seller.
-> An Agent is associated with Transactions.

Primary and foreign keys would be defined to establish these relationships. 



![image](https://github.com/ishanimahajan20/ANALYSIS-OF-AIRBNB-DATA-USING-SQL/assets/134215344/72368252-4062-4c95-9087-3265a9994e74)

# Database Structure:

Database Creation: CREATE DATABASE Airbnb; and use Airbnb; create a database named "Airbnb" and set it as the active database.

# Table Definitions:

Listings Table: Stores information about property listings (e.g., ID, type, room details, price, etc.).

Hosts Table: Contains information about hosts (e.g., ID, name, location, superhost status, etc.).
Availability Table: Manages availability details for listings (e.g., ID, listing ID, available date, minimum and maximum nights).

Reviews Table: Stores reviews for listings (e.g., ID, listing ID, reviewer ID, review date, text, and rating).

# DDL STATEMENTS 

![image](https://github.com/ishanimahajan20/ANALYSIS-OF-AIRBNB-DATA-USING-SQL/assets/134215344/61e1ea97-3076-4bb3-aa26-440c2a423f8e)
![image](https://github.com/ishanimahajan20/ANALYSIS-OF-AIRBNB-DATA-USING-SQL/assets/134215344/f2fb6838-11ac-4525-a837-aaa12b03e1ba)
![image](https://github.com/ishanimahajan20/ANALYSIS-OF-AIRBNB-DATA-USING-SQL/assets/134215344/3cb5bcdd-bbce-476f-aa86-6b779da125e8)
![image](https://github.com/ishanimahajan20/ANALYSIS-OF-AIRBNB-DATA-USING-SQL/assets/134215344/695dcb33-74c5-44ab-b446-2083f60cef4f)
![image](https://github.com/ishanimahajan20/ANALYSIS-OF-AIRBNB-DATA-USING-SQL/assets/134215344/c4b2b731-10b7-46a7-9a05-f3b19a6cf831)

# CREATED VIEW FOR QUERY TO GIVE SIMPLIFY ACCESS TO OTHER :

Listing_host View: Combines data from Listings and Hosts, providing a view with listing details and corresponding host information.

LISTING_REVIEWS View: Combines data from Listings and Reviews, offering a view with listing details and associated reviews.

Avg_rating View: Calculates the average rating for each host based on reviews.

![image](https://github.com/ishanimahajan20/ANALYSIS-OF-AIRBNB-DATA-USING-SQL/assets/134215344/f699b815-e1fd-4944-b276-e824b4b425b5)
![image](https://github.com/ishanimahajan20/ANALYSIS-OF-AIRBNB-DATA-USING-SQL/assets/134215344/02ad62b7-8bd5-48b8-a0f4-f5a8ddf391a0)

The ALTER command in SQL is used to make changes to a table, view, or the entire database. We can add, modify, and drop constraints, columns, and indexes using the ALTER command in SQL.

![image](https://github.com/ishanimahajan20/ANALYSIS-OF-AIRBNB-DATA-USING-SQL/assets/134215344/e80152dd-d4ce-4661-b408-9055bfa6322e)

# DML STATEMENTS

Sample data is inserted into the Listings, Hosts, Availability, and Reviews tables.

![image](https://github.com/ishanimahajan20/ANALYSIS-OF-AIRBNB-DATA-USING-SQL/assets/134215344/cc3b068f-fe35-4de5-a8c0-c6d14526baed)

![image](https://github.com/ishanimahajan20/ANALYSIS-OF-AIRBNB-DATA-USING-SQL/assets/134215344/fa38f507-5ceb-43e1-be53-8ee74014f94a)

![image](https://github.com/ishanimahajan20/ANALYSIS-OF-AIRBNB-DATA-USING-SQL/assets/134215344/35db5e49-f193-4faf-84ee-2a941ae7def7)

![image](https://github.com/ishanimahajan20/ANALYSIS-OF-AIRBNB-DATA-USING-SQL/assets/134215344/4029a597-ad94-49c0-a2a5-4a95ab8e0f6a)

# DQL STATEMENTS 

Various SELECT statements are included, likely for querying and retrieving specific information from the created tables and views.

![image](https://github.com/ishanimahajan20/ANALYSIS-OF-AIRBNB-DATA-USING-SQL/assets/134215344/858d8dca-cc38-4f5d-85c1-3f1d4d795325)

![image](https://github.com/ishanimahajan20/ANALYSIS-OF-AIRBNB-DATA-USING-SQL/assets/134215344/5cf15550-3eb4-4115-bd6d-2548dbf24eff)

![image](https://github.com/ishanimahajan20/ANALYSIS-OF-AIRBNB-DATA-USING-SQL/assets/134215344/bc960ecd-2d51-4df1-8fcd-8294df2d27d8)

![image](https://github.com/ishanimahajan20/ANALYSIS-OF-AIRBNB-DATA-USING-SQL/assets/134215344/e5eb4969-5ce9-4258-96ec-bb0228be1dfe)

![image](https://github.com/ishanimahajan20/ANALYSIS-OF-AIRBNB-DATA-USING-SQL/assets/134215344/4e4d08f4-55f1-4d1c-8ea6-4c0359681ddc)

![image](https://github.com/ishanimahajan20/ANALYSIS-OF-AIRBNB-DATA-USING-SQL/assets/134215344/494ce67b-9bc5-4f8b-b7e1-36b3f9bb1281)

![image](https://github.com/ishanimahajan20/ANALYSIS-OF-AIRBNB-DATA-USING-SQL/assets/134215344/78411be4-1cc5-49a9-936f-50b0208881a1)

# In the query below:

We select the city and property_type columns from the Listings table to identify each property's city and property type.

We use the COUNT(*) function to count the number of properties in each city with each property type.

The result is grouped by city and property_type, allowing you to see property counts for each type in each city.

The query orders the results first by city and then by property_count in descending order. This provides a list of cities with property types sorted by the most prevalent property type within each city.

-> This query will help you determine which cities have the highest number of properties and which property types are popular in each location. It's valuable for market analysis and understanding the diversity of property types available in different cities.

![image](https://github.com/ishanimahajan20/ANALYSIS-OF-AIRBNB-DATA-USING-SQL/assets/134215344/e560d9e7-07c3-474a-ac83-2536184681e0)

# In this query above :

We extract the month from the available_date column in the Availability table.

We calculate the average price for available properties in each month.

The result is grouped by the month, providing insights into seasonal pricing trends.

-> These queries will help you analyze seasonal trends in property availability and pricing, allowing you to identify peak booking periods, high-demand seasons, and pricing variations throughout the year.

![image](https://github.com/ishanimahajan20/ANALYSIS-OF-AIRBNB-DATA-USING-SQL/assets/134215344/05eacb4a-9b2f-4f77-ad7a-5afde6230247)

# In this query:

We calculate the stay duration by finding the difference between the checkout_date and checkin_date using the DATEDIFF function.

We calculate the average review rating (review_rating) for each stay duration.

We use JOIN to link the Booking table with the Reviews table based on the booking_id.

The result is grouped by stay_duration, allowing you to examine how stay duration relates to average review ratings.

The query orders the results by stay_duration in ascending order.

-> This query will help you analyze whether guests tend to leave more positive reviews when they stay for longer periods. You can assess whether there is a correlation between the length of the stay and the average review rating, which can provide insights into guest satisfaction.

![image](https://github.com/ishanimahajan20/ANALYSIS-OF-AIRBNB-DATA-USING-SQL/assets/134215344/8d1bd7c4-dd3b-4978-98db-3cf1c1fb645d)

# In this query:

We use the CORR function to calculate the Pearson correlation coefficient between price and review_rating.

We join the Listings and Reviews tables based on the listing_id to access both price and review rating data.

The result will provide the correlation coefficient, which measures the strength and direction of the linear relationship between pricing and guest ratings.

A positive correlation indicates that higher prices are associated with higher ratings, while a negative correlation suggests that higher prices are associated with lower ratings. A correlation close to zero implies little to no linear relationship.

This query will help you determine whether there is a correlation between pricing and guest ratings, allowing you to assess whether guests are more likely to leave positive reviews for higher-priced listings or vice versa.



# This database offers a rich source of data that can be used to derive valuable business insights. Here are some of the business questions and insights you can explore:

This is not part of project but just to explore more in future!
(SOME OF THE QUESTIONS WE CAN TRY TO WRITE QUERY AS MENTIONED ABOVE)

Host Performance Analysis:

What is the average rating for each host, and how does it correlate with their response time and superhost status?

SELECT
    Host_ID,
    AVG(Rating) AS AverageRating,
    ResponseTime,
    SuperhostStatus
FROM
    Hosts
JOIN
    Ratings ON Hosts.Host_ID = Ratings.Host_ID
GROUP BY
    Host_ID, ResponseTime, SuperhostStatus;

Property Quality Assessment:

What are the common themes in guest reviews, and are there specific areas where hosts can improve?

SELECT Review_text, COUNT(*) AS ReviewCount
FROM Reviews
GROUP BY Review_text
ORDER BY ReviewCount DESC;

for more advanced analysis involving natural language processing, you'd typically use a programming language like Python with specialized libraries (NLTK, spaCy, etc.) and techniques (topic modeling, sentiment analysis) 

Market Analysis:

In which cities are Airbnb properties most prevalent, and what types of properties are popular in each location?

( for this question we need to create a new table as properties , which is currently not in dataset)

SELECT City, PropertyType, COUNT(*) AS PropertyCount
FROM Properties
GROUP BY City, PropertyType
ORDER BY PropertyCount DESC;


















