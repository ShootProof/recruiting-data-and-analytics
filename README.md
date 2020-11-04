# ShootProof Data Analyst
Here at ShootProof, we prefer to have a good idea of a candidate's technical experience and analysis skills before proceeding with portions of our recruiting process. We believe that the exercise below will illustrate a candidate's approach to working with technologies and methodologies that may be commonly used in our data and analytics engineering team here at ShootProof

## Guidelines
-  This exercise should not take you more than two hours to complete. If your solution is taking longer, that's okay—be honest and let us know how long it took and why you think it took that long
- The data is provided as a SQLite Database. Please download the database file and connect using the tools provided below
-   Be as thorough as you wish
-   All exercises are to be performed as if you were on the job
-   Please include both the answer and the SQL code
-  For the Data Visualization portion, there are no right or wrong answers. We are deliberately offering creative freedom and interpretation to all candidates who are completing this exercise. You would receive similar tasks on the job and would be given similar latitude with how you approach the problem and deliver business insights
- The data files in the tables folder included in this .zip can be ignored. These files represent a superset of the data included in the provided SQLite DB and so any SQL answer or data visualization based this data will provide incorrect results

## SQL IDE
DBeaver is an open source SQL IDE that supports SQLite databases

#### DBeaver Download
https://dbeaver.io/download/

#### How to connect to a SQLite Database
https://www.devart.com/odbc/sqlite/docs/index.html?dbeaver.htm

SQLite has a handful of unique quirks. Our intention is not to test your knowledge of SQLite specific syntax. If there is an issue completing a task please share how you would accomplish that task using the SQL syntax you would normally use

One particular SQLite quirk pertains to dates and the fact that this is not a defined datatype. Rather, you will need to leverage SQLite's built-in date and time functions. See below for notes on how to best manage this

[SQLite Documentation](https://www.sqlitetutorial.net/sqlite-date-functions/sqlite-date-function/)

## Tableau Public
A free version of Tableau is available here: [https://public.tableau.com/en-us/s/download](https://public.tableau.com/en-us/s/download)

## ShootProof Data Definitions
**Customer** - A studio in a status of Active or Suspended, on a plan with a value > 0, and no longer in the trial period

**Churn** - A studio that was considered a customer in the previous time period, that is no longer a customer

**Trial Signup** - All studios start as a trial, the signup date is the same date the studio is created

## SQL Assessment

1.  How many customers does ShootProof have?
2.  How many customers are on currently on a plan that allows 5000 photos?
3.  How many trials completed in June 2018?
4.  How many customers did ShootProof have on April 30th, 2020?
5.  How many customers churned between January 1, 2019 and January 1, 2020?

## Data Visualization Assessment

Using a Tableau Public (or Tableau Desktop if you have a license), create a dashboard using the data available. Please limit this portion of the assessment to 1 hour

Hints:
1. Possible items to explore are customer segmentation, customer churn, customer growth, trial conversions, etc.
2. If using Tableau Public, note that it does not support live data connectors. You should export the dataset you intend to use for visualization to either Excel or .csv

## Deliverables

Submission for this exercise should include the following:
1. Text file including SQL for all answers to the SQL Assessment portion of the exercise
2. Link to the Tableau Public dashboard created from the Data Visualization Assessment, or a Tableau workbook file (if using Tableau Desktop)
3. If using an exported .csv or Excel file as your datasource for Tableau, please include these as well as a text file documenting the SQL used to produce the extract
