# nosql-challenge
Module 12 Challenge

NoSQL Challenge
This repository contains the solutions to the NoSQL Challenge provided by Eat Safe, Love magazine for evaluating food hygiene ratings data across the United Kingdom.

Before You Begin
Create a new repository: Create a new repository for this project called nosql-challenge. Do not add this homework to an existing repository.

Clone the repository: Clone the new repository to your computer.

Add necessary files: Add your Jupyter notebook starter files and your Resources folder containing establishments.json to this folder.

Push changes to GitHub: Push the changes to GitHub.

Files
Download the starter code files to help you get started:

Module 12 Challenge files

Instructions
Part 1: Database and Jupyter Notebook Set Up
Use NoSQL_setup_starter.ipynb for this section of the challenge.

Import the data provided in the establishments.json file from your Terminal. Name the database uk_food and the collection establishments. Copy the text you used to import your data from your Terminal to a markdown cell in your notebook.

Within your notebook, import the necessary libraries: PyMongo and Pretty Print (pprint).

Create an instance of the Mongo Client.

Confirm that you created the database and loaded the data properly:

List the databases you have in MongoDB and confirm that uk_food is listed.
List the collection(s) in the database to ensure that establishments is there.
Find and display one document in the establishments collection using find_one() and display with pprint.
Assign the establishments collection to a variable to prepare the collection for use.
Part 2: Update the Database
Use NoSQL_setup_starter.ipynb for this section of the challenge.

The magazine editors have requested some modifications for the database before performing any queries or analysis. Make the following changes to the establishments collection:

Add information about an exciting new halal restaurant named "Penang Flavours" located in Greenwich, which hasn't been rated yet.
Find the BusinessTypeID for "Restaurant/Cafe/Canteen" and return only the BusinessTypeID and BusinessType fields.
Update the new restaurant with the BusinessTypeID found.
Remove any establishments within the Dover Local Authority from the database.
Convert latitude, longitude, and RatingValue to appropriate data types.
Part 3: Exploratory Analysis
Use NoSQL_analysis_starter.ipynb for this section of the challenge.

Explore the dataset to answer specific questions provided by Eat Safe, Love magazine:

Which establishments have a hygiene score equal to 20?
Which establishments in London have a RatingValue greater than or equal to 4?
What are the top 5 establishments with a RatingValue of 5, sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"?
How many establishments in each Local Authority area have a hygiene score of 0? Sort the results from highest to lowest, and print out the top ten local authority areas.
For each question:

Use count_documents to display the number of documents contained in the result.
Display the first document in the results using pprint.
Convert the result to a Pandas DataFrame, print the number of rows in the DataFrame, and display the first 10 rows.
Note
The RatingValue field may contain non-numeric values such as 'Pass'. These values are coerced to nulls during the database setup before converting ratings to integers.
The scores for Hygiene, Structural, and ConfidenceInManagement work in reverse. Higher values indicate worse conditions.
Author
This project was created by Sonal Bhosle.

References used:
- In class activities
- Chat Gpt to validate the codes
- Asked BCS support team Veerance for the mongodb import code and Courtney for No_SQL_Analysis starter question number 3 What are the top 5 establishments with a `RatingValue` rating value of 5, sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"? and 4. How many establishments in each Local Authority area have a hygiene score of 0?
- Referred to youtube : https://youtu.be/c2M-rlkkT5o?si=ELK3xTHABg8-Vg72
