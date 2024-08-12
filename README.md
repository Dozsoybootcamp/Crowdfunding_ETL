
markdown
Copy code
# Crowdfunding Data Analysis Project

## Project Overview
This project aims to analyze crowdfunding campaigns by creating a comprehensive database that includes categories, subcategories, contacts, and campaigns. The goal is to gain insights into the crowdfunding landscape and understand trends based on various parameters.

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [DataFrames](#dataframes)
- [Database Schema](#database-schema)
- [Exported CSV Files](#exported-csv-files)
- [License](#license)

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/Dozsoybootcamp/Crowdfunding_ETL.git
Navigate to the project directory:
bash
Copy code
cd Crowdfunding_ETL
Install the required packages (if using Python):
bash
Copy code
pip install -r requirements.txt
Usage
Run the Python scripts to create DataFrames and populate the database:
bash
Copy code
python main.py
Ensure that your database server is running and configured properly.
DataFrames
Category DataFrame
Columns: category_id, category
Description: Contains unique categories for crowdfunding campaigns.
Subcategory DataFrame
Columns: subcategory_id, subcategory
Description: Contains unique subcategories under each category.
Campaign DataFrame
Columns:
cf_id
contact_id
company_name
description
goal (float)
pledged (float)
outcome
backers_count
country
currency
launch_date (YYYY-MM-DD)
end_date (YYYY-MM-DD)
category_id
subcategory_id
Description: Contains detailed information about each crowdfunding campaign.
Contacts DataFrame
Columns: contact_id, first_name, last_name, email
Description: Contains information about contacts associated with the campaigns.
Database Schema
The database schema is defined in the crowdfunding_db_schema.sql file. It includes the creation of tables with appropriate primary and foreign keys to maintain relationships.

Exported CSV Files
The following CSV files have been exported:

category.csv: Contains category data.
subcategory.csv: Contains subcategory data.
campaign.csv: Contains campaign data.
contacts.csv: Contains contact information.

