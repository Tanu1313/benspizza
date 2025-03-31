## BENS-PIZZA 
BEN'S PIZZA: DATABASE DESIGN, SQL, DATA VISUALIZATION.
##
Overview
##
In the culinary industry, knowing client preferences, controlling inventory, and staffing levels to perfection are essential to a restaurant's success. In order to gather information that informs strategic decision-making, I examine the workings of a hypothetical restaurant called Ben's restaurant in this data analysis case study. I use a visually appealing Tableau Public dashboard to study the complexities of orders, ingredients, pricing, and personnel using SQL.
##
Table Drawing and Data Modelling
##
I start my project by utilising Quick Database Diagrams to sketch tables. The relationships between orders, items, addresses, recipes, ingredients, inventories, staff, rota, and shifts were all carefully considered when I developed the data model. This helped in minimizing Data Redundancy and efficient data organization.
##
![bens](https://github.com/AkshataPatil99/BENS-PIZZA/assets/171495035/4595ff0e-de38-41fa-a5be-a57c21d55dd6)
##
Data Formatting and Table Preparation
##
I used Excel to format the data after sketching to make sure it was accurate and consistent. The carefully chosen tables were then imported into SQL for further examination.
##
Exploratory Data Analysis (EDA) using SQL
##
I started my analysis by delving into the SQL queries that reveal the narrative concealed in the data. These are the main actions and questions that influenced my understanding:
##
Query 1: Order and Sales Insights
##
This illuminates critical sales and order metrics. It offers a comprehensive view of total orders, sales, items sold, average order value, sales by category, top-selling items, orders by hour, sales by hour, and orders by address.
##
![image](https://github.com/AkshataPatil99/BENS-PIZZA/assets/171495035/77085658-f43d-4de7-8d44-31d1350c8e6a)
##
Query 2: Ingredient Insights and Cost Analysis
##
The second query delves into ingredient-level insights, costs, and inventory management. It breaks down total quantity by ingredients, total ingredient cost, calculated pizza cost, and percentage stock remaining by ingredient.
##
![image](https://github.com/AkshataPatil99/BENS-PIZZA/assets/171495035/613b4204-0f93-41f4-954a-41aefa19b9f0)
##
Query 3: Staffing and Cost Management
##
My final query focuses on staffing-related insights, showcasing total staff cost, hours worked, and staff details summary.
##
![image](https://github.com/AkshataPatil99/BENS-PIZZA/assets/171495035/89e6208f-529d-47eb-995e-c99072b540a9)
##
SQL code calculates the total hours worked in a shift and the staff cost for that shift. Here’s a breakdown of the calculations and their purposes:
##
Calculating hours worked (hours_in_shift):
##
TIMEDIFF(sh.end_time, sh.start_time): This function calculates the difference between the shift end time (sh.end_time) and shift start time (sh.start_time).
##
TIME_TO_SEC(...): This function converts the time difference to seconds.
##
/ 3600: This converts the time in seconds to hours (since 1 hour = 3600 seconds).
##
Calculating staff cost (staff_cost):
##
The result of the hours worked calculation (TIME_TO_SEC(TIMEDIFF(sh.end_time, sh.start_time)) / 3600).
##
Multiplied by the hourly rate (s.hourly_rate).
##
Tableau Public: A Visual Journey
##
My analysis of Ben’s Pizzeria extended to Tableau Public, where I crafted a dynamic dashboard that presents data in visually engaging ways. While the intricate SQL queries laid the groundwork for my insights, the Tableau Public complements the analysis by providing a holistic view of key metrics.
##
Dashboard 1 — Orders
##
My first Tableau Public dashboard offers a visual representation of order-related insights. It highlights metrics like total orders, total sales, total items, and average order value. The pie chart showcases sales distribution by product, and the bar graph illustrates total sales by product subcategory.The hourly line graph displays the flow of total orders and sales over time. 
##
![bens_orders](https://github.com/AkshataPatil99/BENS-PIZZA/assets/171495035/15139065-492a-4c2e-8c29-13085265e454)
##
Dashboard 2 — Inventory
##
The second Tableau Publi dashboard delves into inventory-related metrics. It visualizes ingredient costs, total quantity, total cost, and the percentage of remaining inventory. Additionally, it presents the cost of each item by calculating the ingredient cost. These visualizations empower the team to monitor inventory health and make informed decisions about ingredient procurement and usage.
##
![bens_inv](https://github.com/AkshataPatil99/BENS-PIZZA/assets/171495035/70d75919-1d4c-44ef-a1ac-80a446a89412)
##
Dashboard 3 — Staff
##
The third Tableau Public dashboard provides insights into staffing costs and hours worked. Visualizing staff costs, total hours worked, and other staffing details aids in optimizing workforce management. This visual summary assists in aligning staffing resources with peak hours of operation.
##
![bens_staff](https://github.com/AkshataPatil99/BENS-PIZZA/assets/171495035/01bd7c67-f888-4af6-8c61-21fe7447cd75)
##
A Comprehensive Method: Analyzing and Visualizing Data
##
The combination of Tableau visualizations and SQL analysis results in a thorough method for extracting insights. The narrative of  the data is carefully revealed by the SQL queries, and it is presented in aesthetically pleasing and easily comprehensible formats by the Tableau dashboards. Decision-makers at Ben's Pizzeria are now able to act strategically thanks to this combined approach, which gives them a complete grasp of sales trends, ingredient costs, staffing efficiency, and other factors.

