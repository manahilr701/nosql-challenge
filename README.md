# NoSQL Challenge - UK Food Standards Agency Data

## Project Overview

This project involves working with the UK Food Standards Agency data to analyze food hygiene ratings of establishments across the United Kingdom. The goal is to assist the food magazine *Eat Safe, Love* by evaluating the hygiene data, enabling their journalists and food critics to focus on notable establishments.

The project is divided into two main parts:
- **Part 1**: Database Setup and Data Import
- **Part 2**: Database Modifications and Exploratory Data Analysis

## Prerequisites

To run this project, ensure that you have the following installed:

- MongoDB
- Python 3.x
- Python Libraries: `pymongo`, `pandas`, `pprint`

You can install the required Python libraries using the following command:

```bash
pip install pymongo pandas

## Database Connection

A connection to the MongoDB instance was established using pymongo, and the data import was verified.

## Verification of Data

The notebook lists the databases and collections, confirming the presence of the uk_food database and establishments collection.

# Part 2: Database Modifications and Updates

## Key Tasks:
- Insert New Restaurant: Added a new restaurant called Penang Flavours to the collection.
- Update BusinessTypeID: The BusinessTypeID for Penang Flavours was updated to match the Restaurant/Cafe/Canteen type.
- Remove Dover Establishments: All establishments in Dover were removed from the collection.
- Convert String to Numeric: Converted RatingValue from a string to an integer where applicable, and converted latitude/longitude to decimal numbers.
- Part 3: Exploratory Data Analysis
- The following queries were conducted to provide insights:

Establishments with a Hygiene Score of 20: Identified establishments with a hygiene score of 20.
London Establishments with High Ratings: Found establishments in London with a RatingValue of 4 or higher.
Top 5 Establishments Near "Penang Flavours": Found the top 5 establishments with a RatingValue of 5, located closest to Penang Flavours and sorted by hygiene score.
Establishments with a Hygiene Score of 0: Counted establishments with a hygiene score of 0 across different local authorities.
How to Use
Clone the Repository
bash
Copy code
git clone <your-repo-url>
cd nosql-challenge
Set Up MongoDB
Ensure that MongoDB is running on your local machine, and import the data using the mongoimport command:

bash
Copy code
mongoimport --db uk_food --collection establishments --drop --file establishments.json --jsonArray
Run Jupyter Notebooks
Open the notebooks and run the cells:

bash
Copy code
jupyter notebook
Execute the Code
Follow the instructions within the notebooks to perform the database setup and data analysis.

Results
The analysis provides insights into food hygiene ratings across various UK establishments, assisting the magazine with identifying noteworthy locations for their articles.

License
This project is licensed under the MIT License.

