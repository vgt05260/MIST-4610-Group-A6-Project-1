# MIST-4610-Group-A6-Project-1
UGA MIST 4610 Group Project for Professor Marie-Claude Boudreau

# Group Information
Group A6
- Group Leader: Victoria Taylor
- Conceptual Modeler:
- Database Designer: Rishi Patel
- Data Wrangler:
- SQL Writer:

# Case Description
Case#3 – The Peach State Film Festival

Peach State Film Festival (PSFF) is a week-long festival hosted across multiple theaters in Atlanta, Georgia. PSFF
wants to develop a database to manage film submissions, screenings, and volunteer staffi

# Data Model
The data model png is in the Project Diagram.png in this repository.

# Data Dictionary
The data dictionary pdf if in the Data Dictionary.pdf in this repository.

# Ten Queries
## Query 1
Query 1 lists the titles, runtimes, languages, countries, and ratings of films that are rated PG or PG-13, ordered from longest to shortest runtime.
<img width="2048" height="574" alt="image" src="https://github.com/user-attachments/assets/895fc352-56ac-48c1-bee1-a757064c8c96" />
### Managerial Justification
This query is useful for identifying family-friendly or broadly accessible films within the festival lineup while also highlighting their relative lengths. Festival organizers can use this information to better schedule screenings, ensuring that longer films are placed in appropriate time slots and that audiences interested in PG or PG-13 content can easily find suitable options. Additionally, understanding the distribution of these films by language and country can help with programming diversity and audience targeting.
### Technical Justification
This query demonstrates basic SELECT-FROM-WHERE structure, along with filtering conditions and ORDER BY sorting. It reinforces foundational SQL skills such as selecting specific columns, applying conditions to narrow results, and organizing output in a meaningful order.

## Query 2
Query 2 lists the category names, submission fees, and runtime limits for categories with submission fees greater than 20 dollars, ordered from highest to lowest fee.
<img width="2047" height="573" alt="image" src="https://github.com/user-attachments/assets/7ffb553e-0608-4a09-93a7-3bd6c42a5526" />
### Managerial Justification
This query is useful for understanding which film categories generate the most revenue through submission fees and how those categories are structured in terms of runtime expectations. Festival organizers can use this information to evaluate pricing strategies, identify premium categories, and ensure that higher-cost submissions align with longer or more competitive film formats. It also helps in assessing whether submission fees are appropriately scaled relative to category requirements and perceived value.
### Technical Justification
This query demonstrates filtering numeric data and sorting results, reinforcing the use of comparison operators and ORDER BY. It also shows understanding of working with standalone tables and extracting relevant attributes for analysis.

## Query 3
Query 3 lists each reservation’s ID, date and time, reserved seats, and the first and last name of the customer who made the reservation, ordered chronologically by reservation date and time.
<img width="2048" height="612" alt="image" src="https://github.com/user-attachments/assets/ef4f5839-95d4-4b28-b33b-b7a0d76db4aa" />
### Managerial Justification
This query is useful for tracking booking activity and linking each reservation to the corresponding customer. Festival organizers can use this information to monitor attendance patterns, identify peak reservation times, and manage seating logistics more effectively. Additionally, having customer names associated with reservations allows staff to quickly verify bookings, assist attendees, and maintain accurate records for customer service and event planning purposes.
### Technical Justification
This query demonstrates a two-table join using a foreign key relationship between reservation and customer. It reinforces understanding of table relationships, aliasing, and combining data from multiple tables, along with sorting results.

## Query 4
Query 4 lists the first and last names of customers along with their reservation IDs for reservations that have been checked in, ordered alphabetically by last name.
<img width="2048" height="664" alt="image" src="https://github.com/user-attachments/assets/920d4db0-f936-490e-9910-fb4293492350" />
### Managerial Justification
This query is useful for identifying which customers have successfully checked in to their reserved screenings, allowing event staff to monitor attendance and verify entry in real time. By organizing the results alphabetically, staff can quickly locate individuals when assisting with inquiries or resolving issues at check-in. Additionally, this information can help organizers analyze attendance rates, compare reservations to actual turnout, and improve future event planning and capacity management.
### Technical Justification
This query builds on join logic by adding multiple filtering conditions, including a Boolean/flag field (reservation_checkin). It demonstrates combining JOIN + WHERE conditions, and sorting by a different attribute, reinforcing more complex query construction.

## Query 5
Query 5 lists each volunteer’s first and last name along with the date, start time, end time, and role of the shifts they are assigned to, ordered by shift date and volunteer last name.
<img width="2048" height="627" alt="image" src="https://github.com/user-attachments/assets/670272d0-8b52-4175-a4d7-80fe4206d834" />
### Managerial Justification
This query is useful for managing volunteer scheduling and ensuring that all shifts are properly staffed. Festival coordinators can use this information to view who is assigned to each shift, verify role coverage, and identify any scheduling gaps or overlaps. Additionally, organizing the results by date and volunteer name makes it easier to coordinate daily operations, communicate assignments to volunteers, and maintain an efficient and well-structured event workflow.
### Technical Justification
This query demonstrates a three-table join, combining volunteer, assignment, and volunteer_shift. It reinforces understanding of junction tables, multi-step relationships, and retrieving structured scheduling data. It also shows ordering by multiple columns.

## Query 6
Query 6 lists each film country along with the number of distinct films from that country and the total number of screenings those films have, ordered from highest to lowest number of films.
<img width="2048" height="679" alt="image" src="https://github.com/user-attachments/assets/c5fda2aa-e8f7-4627-b2a7-51a4815732ea" />
### Managerial Justification
This query is useful for analyzing the geographic distribution of films in the festival and understanding how representation from each country translates into screening frequency. Festival organizers can use this information to evaluate diversity in programming, identify countries with strong participation, and assess whether certain regions are receiving more exposure through screenings. This insight can support decisions related to future outreach, partnerships, and balancing international representation in the festival lineup.
### Technical Justification
This query demonstrates aggregation using COUNT(), DISTINCT, and GROUP BY. It also combines aggregation with a join between film and screening, reinforcing how to summarize data across related tables and sort aggregated results.

## Query 7
Query 7 lists each film’s title, rating, runtime, the submitter’s first and last name, and the category name and submission fee it belongs to, ordered by category and film title.
<img width="2048" height="575" alt="image" src="https://github.com/user-attachments/assets/0efebb82-1090-47a7-bbb1-0969157c1097" />
### Managerial Justification
This query is useful for understanding how films are distributed across categories and who submitted them, while also providing insight into the financial and structural aspects of each category. Festival organizers can use this information to track submissions, evaluate participation by category, and ensure proper organization of films within the program. Additionally, linking films to submitters and submission fees helps support administrative tasks such as billing, reporting, and assessing which categories attract the most entries.
### Technical Justification
This query demonstrates a three-table join across film, submitter, and category, reinforcing understanding of multiple foreign key relationships. It also shows selecting attributes from different entities and organizing results with ORDER BY on multiple fields.

## Query 8
Query 8 lists paired films by showing the title of each film in the pair, along with the pairing type and the date the pairing was established, ordered by pairing date.
<img width="2048" height="652" alt="image" src="https://github.com/user-attachments/assets/b3559c60-ac1e-49e1-bc9f-b64112971548" />
### Managerial Justification
This query is useful for understanding how films are intentionally grouped within the festival program, such as double features or thematic pairings. Festival organizers can use this information to coordinate scheduling, marketing, and audience experience by highlighting curated film combinations. Additionally, tracking pairing types and dates helps ensure proper documentation of programming decisions and allows for analysis of how different pairing strategies are used throughout the festival.
### Technical Justification
This query demonstrates a self-join pattern by referencing the film table twice (aliased as f1 and f2) through the pairing table. It reinforces the concept of recursive/relational relationships within the same entity, along with aliasing and joining multiple instances of a table.

## Query 9
Query 9 lists each film along with its shooting location (location name, city, and country), and classifies the film’s origin as “Local - Georgia,” “Domestic - Other State,” or “International” based on the location’s state/province and country. Results are ordered first by the derived origin category and then alphabetically by film title.
<img width="2048" height="784" alt="image" src="https://github.com/user-attachments/assets/49057f31-e62d-47ad-ae08-356670e1f88e" />
### Managerial Justification
This query provides management with a clear breakdown of where films in the festival are being produced relative to Georgia. By identifying which films are locally produced, from other U.S. states, or international, festival organizers can evaluate how well they are supporting local filmmakers versus attracting broader submissions. This insight can inform strategic decisions such as allocating marketing efforts, adjusting submission incentives, prioritizing local partnerships, or demonstrating regional economic impact to sponsors and stakeholders.
### Technical Justification
This query demonstrates the use of a CASE statement to create a derived attribute (film_origin) based on multiple conditions, as well as a three-table join (film, shoot_details, and location) to combine related data. It also shows handling of non-standard column names using backticks and reinforces sorting by both a computed field and a base column. This reflects practical SQL use for categorization and reporting.

## Query 10
Query 10 lists each venue along with the number of employee shifts, total labor cost (rounded to two decimal places), and number of volunteer shifts associated with that venue. Results are grouped by venue and ordered by total labor cost in descending order.
<img width="2048" height="741" alt="image" src="https://github.com/user-attachments/assets/2a0f8d55-f709-4ee9-806a-da13f52c65de" />
### Managerial Justification
This query provides festival management with a clear comparison of staffing levels and labor costs across venues. By analyzing both paid employee shifts and volunteer contributions, decision-makers can assess operational efficiency, identify high-cost venues, and determine whether staffing resources are being allocated effectively. This insight supports budgeting decisions, workforce planning, and optimization of volunteer versus paid labor distribution.
### Technical Justification
This query demonstrates aggregation functions including COUNT(DISTINCT) and SUM, as well as ROUND for formatting numeric output. It uses a three-table join (venue, employee_shift, volunteer_shift) to combine related operational data, and applies GROUP BY to aggregate results at the venue level. It also reinforces sorting by a computed column (total_labor_cost) and handling multiple aggregates within a single query.

# Database Information
Name of the database: mb_A6
Additional information: Each query listed above is marked in the database using stored procedures which can be called using the following format: CALL GP_Q1();
