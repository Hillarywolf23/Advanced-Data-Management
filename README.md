# Advanced-Data-Management
WGU D326 Performance Assessment Project

# DVD Database Business Report Project

## Overview
This project simulates a common data analyst task: transforming and reporting on data stored in a relational database so that it can be easily understood and used by both technical and nontechnical stakeholders. Using the DVD Database from the Labs on Demand Assessment Environment, the project demonstrates how to answer a real-world business question by creating two types of report sections:

- **Detailed Table:** Contains granular, transaction-level data that informs the analysis.
- **Summary Table:** Provides aggregated data that directly answers the business question.

By leveraging SQL functions, triggers, and stored procedures, this project automates data transformation and report refresh processes, ensuring that the resulting business report is both comprehensive and current.

## Project Objectives
- **Data Transformation:** Convert raw data from the DVD Database into a format that is useful for business analysis.
- **Report Segmentation:** 
  - **Detailed Section:** Present all relevant data at a fine level of granularity.
  - **Summary Section:** Aggregate the detailed data to deliver clear, actionable insights.
- **Automation:** Develop SQL code (functions, triggers, and stored procedures) to:
  - Transform data fields as needed (e.g., translating binary values like `N`/`Y` into human-readable text such as "No" and "Yes").
  - Automatically update the summary table when new data is inserted into the detailed table.
  - Refresh both report sections on a regular schedule.
- **Business Reporting:** Create a business report that answers a specific business question using real data from the DVD Database.

## Project Components
1. **Detailed Table:**
   - **Data Fields:** Contains selected fields from at least two tables in the DVD Database.
   - **Custom Transformation:** Includes at least one field that is transformed via a user-defined function (e.g., converting a binary indicator to a more descriptive value).

2. **Summary Table:**
   - **Aggregated Data:** Provides a high-level view that directly addresses the chosen business question.
   - **Real-Time Updates:** Designed to be updated automatically through a trigger whenever the detailed table is modified.

3. **SQL Functions:**
   - Custom function(s) perform specific data transformations (such as mapping `N` to "No" and `Y` to "Yes").

4. **SQL Trigger:**
   - Automatically updates the summary table whenever new rows are added to the detailed table, ensuring consistency between the two sections.

5. **Stored Procedure:**
   - Clears and refreshes both the detailed and summary tables by re-extracting raw data from the DVD Database.
   - Intended for scheduled execution using a job scheduling tool (e.g., cron or pgAgent) to keep the report current.

6. **Business Report & Demonstration:**
   - **Business Report:** A written summary that explains the business question, the data used, and the insights derived from both the detailed and summary tables.
   - **Panopto Video:** A recorded demonstration featuring a walkthrough of the code and its functionality, providing context and insight into the report’s construction.

## Business Use Cases
- **Detailed Table:** Serves as the foundation for in-depth analysis, allowing analysts to drill down into individual transactions and trends.
- **Summary Table:** Offers decision-makers a high-level view of performance, trends, or anomalies—enabling faster, more informed business decisions.

## Report Refresh Strategy
- **Real-Time Updates:** A trigger ensures that any new data added to the detailed table is immediately reflected in the summary table.
- **Scheduled Refreshes:** The stored procedure is designed to run on a regular schedule (such as nightly or weekly) to ensure that both the detailed and summary tables contain the most recent data. Tools like **cron** or **pgAgent** can be used for this purpose.

## Getting Started
1. **Environment Setup:**  
   - Access the Labs on Demand Assessment Environment.
   - Connect to the DVD Database provided in the environment.

2. **Executing the Code:**  
   - Run the SQL scripts to create the detailed and summary tables.
   - Create and test the custom SQL functions, triggers, and stored procedures.
   - Execute the SQL query to extract raw data for the detailed report section.

3. **Reviewing the Demonstration:**  
   - Watch the Panopto video demonstration to see the functionality of the code in action.

## Acknowledgments
- All code provided in this project is original and developed for this assignment.
- No external sources were directly used for the code; all references are based on the project instructions and standard SQL practices.

## Contact
For questions or further information regarding this project, please contact the project author.
