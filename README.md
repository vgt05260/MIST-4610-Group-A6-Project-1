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
This query is useful for identifying family-friendly or broadly accessible films within the festival lineup while also highlighting their relative lengths. Festival organizers can use this information to better schedule screenings, ensuring that longer films are placed in appropriate time slots and that audiences interested in PG or PG-13 content can easily find suitable options. Additionally, understanding the distribution of these films by language and country can help with programming diversity and audience targeting.

## Query 2
Query 2 lists the category names, submission fees, and runtime limits for categories with submission fees greater than 20 dollars, ordered from highest to lowest fee.
<img width="2047" height="573" alt="image" src="https://github.com/user-attachments/assets/7ffb553e-0608-4a09-93a7-3bd6c42a5526" />
This query is useful for understanding which film categories generate the most revenue through submission fees and how those categories are structured in terms of runtime expectations. Festival organizers can use this information to evaluate pricing strategies, identify premium categories, and ensure that higher-cost submissions align with longer or more competitive film formats. It also helps in assessing whether submission fees are appropriately scaled relative to category requirements and perceived value.

## Query 3
Query 3 lists each reservation’s ID, date and time, reserved seats, and the first and last name of the customer who made the reservation, ordered chronologically by reservation date and time.
<img width="2048" height="612" alt="image" src="https://github.com/user-attachments/assets/ef4f5839-95d4-4b28-b33b-b7a0d76db4aa" />
This query is useful for tracking booking activity and linking each reservation to the corresponding customer. Festival organizers can use this information to monitor attendance patterns, identify peak reservation times, and manage seating logistics more effectively. Additionally, having customer names associated with reservations allows staff to quickly verify bookings, assist attendees, and maintain accurate records for customer service and event planning purposes.

## Query 4
Query 4 lists the first and last names of customers along with their reservation IDs for reservations that have been checked in, ordered alphabetically by last name.
<img width="2048" height="664" alt="image" src="https://github.com/user-attachments/assets/920d4db0-f936-490e-9910-fb4293492350" />
This query is useful for identifying which customers have successfully checked in to their reserved screenings, allowing event staff to monitor attendance and verify entry in real time. By organizing the results alphabetically, staff can quickly locate individuals when assisting with inquiries or resolving issues at check-in. Additionally, this information can help organizers analyze attendance rates, compare reservations to actual turnout, and improve future event planning and capacity management.

## Query 5
Query 5 lists each volunteer’s first and last name along with the date, start time, end time, and role of the shifts they are assigned to, ordered by shift date and volunteer last name.
<img width="2048" height="627" alt="image" src="https://github.com/user-attachments/assets/670272d0-8b52-4175-a4d7-80fe4206d834" />
This query is useful for managing volunteer scheduling and ensuring that all shifts are properly staffed. Festival coordinators can use this information to view who is assigned to each shift, verify role coverage, and identify any scheduling gaps or overlaps. Additionally, organizing the results by date and volunteer name makes it easier to coordinate daily operations, communicate assignments to volunteers, and maintain an efficient and well-structured event workflow.

## Query 6


# Database Information
