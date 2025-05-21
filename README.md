# Help Desk Report
[Visualization on Tableau Public](https://public.tableau.com/app/profile/justinluzong/viz/HelpDeskReport_17477109774400/HelpDeskReport)

## Project Overview
WIP

Insights and recommendations are provided for the following key areas:
- **WIP:** WIP


## Data Structure Overview
The help desk ticket data consists of one table as seen below. The data extracted for this project spans from March 2020 to October 2020, with a total row count of 9,542 records.  

IMAGE WIP


## Executive Summary
WIP


## Insights Deep Dive
### WIP
- WIP  
IMAGE WIP

### WIP
- WIP  
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
- **Owner Group:** This column is assumed to be equivalent to an 'assignment group', the group who will be working on the request.
- **Days Open:** By adding Days Open to the Created Date of the newest Open tickets, the latest date in the dataset is found to be 12/5/2020.
- **Ticket Status:** The open ticket statuses are considered to be 'Open' and 'Waiting for Requestor Feedback' (example: request requires additional information from the user.) A ticket is changed to 'Closed - Incomplete' if the ticket is in an open status and the resulting date of Created Date + Days Open is earlier than the latest date in the dataset, 12/5/2020.
- **Closed Date:** The Closed Date column is also calculated by adding the value of Days Open to the Created Date. The value is NULL if the ticket is in an open status.
- **Satisfaction Score:** Score values have been converted to integers. The range of scores is 1 (lowest) to 3 (highest). Records are given a NULL value if they originally had a score of '0 - Unknown' or are in 'Open', 'Waiting for Requestor Feedback', or 'Closed - Incomplete' status.
