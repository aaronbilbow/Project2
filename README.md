# Crowdfunding Data Processing Project

## Table of Contents

- [Introduction](#introduction)
- [Prerequisites](#prerequisites)
- [Create the Category and Subcategory DataFrames](#create-the-category-and-subcategory-dataframes)
- [Create the Campaign DataFrame](#create-the-campaign-dataframe)
- [Create the Contacts DataFrame](#create-the-contacts-dataframe)
- [Create the Crowdfunding Database](#create-the-crowdfunding-database)
- [Contributing](#contributing)

## Introduction

This project focuses on processing and transforming data from a crowdfunding dataset in Excel format (`crowdfunding.xlsx`). It includes creating DataFrames for categories, subcategories, campaigns, and contacts. Each section below outlines the steps to create the respective DataFrames from the provided Excel data.

## Prerequisites

Before getting started with this project, make sure you have the following prerequisites:

- Python (version 3.6 or higher) https://www.python.org/downloads/
- Pandas library https://pypi.org/project/pandas/#files
- Regex understanding https://www.w3schools.com/python/python_regex.asp
- Basic understanding of data manipulation and Pandas https://pandas.pydata.org/docs/user_guide/10min.html
- PostGres SQL knowledge https://www.postgresql.org/download/

## Create the Category and Subcategory DataFrames

We will begin by creating DataFrames for categories and subcategories:

1. Extract and transform data from `crowdfunding.xlsx` to create a "Category DataFrame" that includes:
   - "category_id" with entries like "cat1", "cat2", etc.
   - "category" containing category titles.
2. Export the Category DataFrame as `category.csv` and save it to your GitHub repository.

3. Similarly, create a "Subcategory DataFrame" with:
   - "subcategory_id" following the pattern "subcat1", "subcat2", etc.
   - "subcategory" with subcategory titles.
4. Export the Subcategory DataFrame as `subcategory.csv` and save it to your GitHub repository.

## Create the Campaign DataFrame

Next, we will create a Campaign DataFrame:

1. Extract and transform data from `crowdfunding.xlsx` to create a DataFrame with columns:
   - "cf_id"
   - "contact_id"
   - "company_name"
   - "description" (renamed from "blurb")
   - "goal" (as float)
   - "pledged" (as float)
   - "outcome"
   - "backers_count"
   - "country"
   - "currency"
   - "launch_date" (converted to datetime)
   - "end_date" (converted to datetime)
   - "category_id" (matching "category_id" from Category DataFrame)
   - "subcategory_id" (matching "subcategory_id" from Subcategory DataFrame)

2. Reorder the columns based on the provided order.
3. Export the Campaign DataFrame as `campaign.csv` and save it to your GitHub repository.

## Create the Contacts DataFrame

## Option 1: Extract and Transform Data Using Python Dictionary Methods

This option involves the following steps:

1. Import the `contacts.xlsx` file into a DataFrame.
2. Iterate through the DataFrame, converting each row to a dictionary.
3. Extract and store the dictionary values for each row.
4. Create a new DataFrame containing the extracted data.
5. Split each "name" column value into first and last names.
6. Clean and export the DataFrame as `contacts.csv`.

## Option 2: Extract and Transform Data Using Regular Expressions

This option involves the following steps:

1. Import the `contacts.xlsx` file into a DataFrame.
2. Extract the "contact_id," "name," and "email" columns using regular expressions.
3. Create a new DataFrame with the extracted data.
4. Convert the "contact_id" column to the integer type.
5. Split each "name" column value into "first_name" and "last_name" columns.
6. Clean and export the DataFrame as `contacts.csv`.

## Create the Contacts DataFrame

Follow these steps to create the Contacts DataFrame using Option 2:

1. Run the Python script that corresponds to Option 2.
2. The script will use regular expressions to extract and transform the data.
3. The "contact_id" column will be converted to integers.
4. The "name" column will be split into "first_name" and "last_name."
5. The resulting DataFrame will be exported as `contacts.csv`.
6. Save the `contacts.csv` file to your GitHub repository.

## Create the Crowdfunding Database



## Contributing

Praveen Kumar Rachakonda, https://github.com/pkrachakonda , 
Aaron Bilbow, https://github.com/aaronbilbow , 
John Poretta, https://github.com/Johnporretta


