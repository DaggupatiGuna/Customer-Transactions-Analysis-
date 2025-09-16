Customer Transactions Analysis
📝 Overview
This repository contains a data pipeline workflow built with KNIME Analytics Platform for a Customer Transactions Analysis project. The workflow was developed to help a sales team member, Pauline, automate her monthly data reporting and visualization tasks. The project provides a complete solution for processing customer transaction data from various sources to generate actionable insights.

🚀 Features
The workflow addresses the full data analysis lifecycle, which is represented by the following key steps:


Data Access 

: The workflow reads data from multiple sources, including:


CustomerInfoSystem1.xlsx and CustomerInfoSystem2.table 


Stores.csv 

Database tables 

Transactions and ProductNrAndPrice 


Data Cleaning and Transformation 

: The data is prepared for analysis by:

Removing duplicate rows based on 

CustomerID.

Handling missing age values by inserting the mean age of the dataset.

Creating a new 

AgeGroup column with values like "Adolescent," "Adult," and "Older Adult".

Splitting the 

CustomerID column and renaming the resulting columns.

Merging the 

Email and CorporateEmail columns.


Data Merging and Aggregation 

: The cleaned data is combined and summarized to get the desired results:

Two customer tables are concatenated.


StoreType and Price information are appended to the transactions data.

Customer and transaction tables are joined on the 

CustomerID column.

Data is aggregated to calculate the total price per customer and the basket size per order.


Data Visualization and Reporting 

: The final insights are visualized and exported:

The total price per customer is written to an Excel file.

A bar chart visualizes the number of orders for each basket size for both online and onsite stores.

An interactive dashboard is created with a scatter plot, bar chart, and parallel coordinates plot to show relationships between various customer and transaction metrics.

The interactive view of the component is rearranged using the Layout Editor.

A PDF report is generated from the dashboard view.

🛠️ How to Use
Ensure you have KNIME Analytics Platform installed.

Clone this repository to your local machine.

Open the Customer Transactions Analysis by Guna.knwf file in KNIME.

Execute the nodes in the workflow to see the data pipeline in action and reproduce the results.
