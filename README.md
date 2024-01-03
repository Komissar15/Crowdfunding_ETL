Project Overview - Crowdfunding ETL

Team Members:


Introduction:
In this project, our team implemented an Extract, Transform, Load (ETL) pipeline using Python and Pandas, employing either Python dictionary methods or regular expressions to extract and transform data. Subsequently, we created four CSV files, constructed an Entity-Relationship Diagram (ERD), developed a table schema, and uploaded the CSV data into a Postgres database.

Instructions:

Create the Category and Subcategory DataFrames:

Extract and transform data from crowdfunding.xlsx to create a category DataFrame with columns: "category_id" (sequential from "cat1" to "catn") and "category" (containing category titles).

Export the category DataFrame as category.csv and save it to the GitHub repository.

Extract and transform data from crowdfunding.xlsx to create a subcategory DataFrame with columns: "subcategory_id" (sequential from "subcat1" to "subcatn") and "subcategory" (containing subcategory titles).

Export the subcategory DataFrame as subcategory.csv and save it to the GitHub repository.

Create the Campaign DataFrame:

Extract and transform data from crowdfunding.xlsx to create a campaign DataFrame with columns including "cf_id," "contact_id," "company_name," "description," "goal," "pledged," "outcome," "backers_count," "country," "currency," "launch_date," "end_date," "category_id," and "subcategory_id."

Convert relevant columns to appropriate data types and format date columns.

Export the campaign DataFrame as campaign.csv and save it to the GitHub repository.

Create the Contacts DataFrame:

Option 1: Use Python dictionary methods.

Import contacts.xlsx into a DataFrame.
Iterate through the DataFrame, converting each row to a dictionary.
Extract values from keys using Python list comprehension.
Create a new DataFrame with the extracted data.
Split "name" column into first and last names.
Clean and export the DataFrame as contacts.csv to the GitHub repository.
Option 2: Use regular expressions.

Import contacts.xlsx into a DataFrame.
Extract "contact_id," "name," and "email" columns using regular expressions.
Create a new DataFrame with the extracted data.
Convert "contact_id" column to integer type.
Split "name" column into first and last names.
Clean and export the DataFrame as contacts.csv to the GitHub repository.
Create the Crowdfunding Database:

Inspect CSV files and sketch an ERD using QuickDBD.
Use ERD information to create a table schema in crowdfunding_db_schema.sql, saved to the GitHub repository.
Create a new Postgres database named crowdfunding_db.
Create tables in the correct order to handle foreign keys based on the schema.
Verify table creation with SELECT statements.
Import each CSV file into its corresponding SQL table.
Verify data correctness with SELECT statements for each table.