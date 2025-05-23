# Help Desk Report
[Visualization on Tableau Public](https://public.tableau.com/app/profile/justinluzong/viz/HelpDeskReport_17477109774400/HelpDeskReport)

## Project Overview
WIP

Insights and recommendations are provided for the following key areas:
- **Issue Trends:** Identification of notable issue categories, owner groups, and severities
- **Mean Time to Resolution (MTTR):** Assessment of the average time required to resolve issues
- **Satisfaction Scores:** Evaluation of score trends, both overall and among various types of issues


## Data Structure Overview
The help desk ticket data consists of one table as seen below. The data extracted for this project spans from March 2020 to October 2020, with a total row count of 9,542 records.  

<img src=https://github.com/user-attachments/assets/a2ff6396-1d24-483f-b548-accd869b48dd width="250">


## Executive Summary
WIP


## Insights Deep Dive
### Issue Category
- The issue category with the largest amount of tickets is Access/Login (3453 tickets, 36.2%)  
IMAGE WIP

### Issue Severity
- WIP  
IMAGE WIP

### Owner Groups
- WIP  
IMAGE WIP

### Mean Time to Resolution (MTTR)
- The overall MTTR across the dataset for resolved tickets is 19.4 days.
- Across months, MTTR doubles from March 2020 (10.1 Days) to April 2020 (20.2).
- MTTR stays relatively stable between April and October (18 ~ 20 Days), then nearly doubles from October (19.0) to December (35.7).  
IMAGE WIP

### Satisfaction Scores 
- The overall average satisfaction score across the dataset is 2.2 out of 3.
- Customers left satisfaction scores on 41.7% of all resolved tickets.
- The average satisfaction score stays relatively stable across months (ranges from 2.0 - 2.3), only changing by .1-.2 points between months.
IMAGE WIP


## Recommendations
### WIP
- **WIP:** WIP

### WIP
- **WIP:** WIP


## Technical Details
Technical analysis for this project involved:
- **Tableau Public:** For data transformation and exploratory data analysis (EDA) via interactive dashboards.

[Visualization on Tableau Public](https://public.tableau.com/app/profile/justinluzong/viz/HelpDeskReport_17477109774400/HelpDeskReport)


## Caveats and Assumptions
This project uses Mark Bradbourne's [Real World Fake Data "Help Desk" dataset](https://data.world/markbradbourne/rwfd-real-world-fake-data/workspace/file?filename=Help+Desk.csv)
- **Severity:** Tickets with '0 - Unassigned' severity are assumed to not have any impact and do not warrant an actual severity value being assigned to them.
- **Owner Group:** The value for this column is assumed to the 'assignment group', the group who will be working on the request.
- **Days Open:** By adding Days Open to the Created Date of the newest Open tickets, the latest date in the dataset is found to be 12/5/2020.
- **Ticket Status:** The open ticket statuses are defined as 'Open' and 'Waiting for Requestor Feedback' (example: request requires additional information from the user.) A ticket's status is updated to 'Closed - Incomplete' if the ticket is in an open status and the resulting date of Created Date + Days Open is earlier than the latest date in the dataset, 12/5/2020.
- **Closed Date:** This column is also calculated by adding the value of Days Open to the Created Date. The value is NULL if the ticket is in an open status.
- **Satisfaction Score:** Score values have been converted to integers. The range of scores is 1 (lowest) to 3 (highest). Records are given a NULL value if they originally had a score of '0 - Unknown' or are in 'Open', 'Waiting for Requestor Feedback', or 'Closed - Incomplete' status.
