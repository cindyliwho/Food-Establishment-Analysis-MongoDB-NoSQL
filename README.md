# UK Food Establishments Analysis (MongoDB / NoSQL)

## Overview
This project uses **MongoDB** and **PyMongo** to store, clean, and analyze food establishment inspection data from the UK. It demonstrates how NoSQL databases can be used for flexible data storage and how MongoDB queries and aggregations can support real-world analytical questions.

The project is split into two notebooks:
1. **Database setup and data preparation**
2. **Exploratory analysis using MongoDB queries**

---

## Dataset
The dataset contains information on UK food establishments, including:
- Business name and type
- Hygiene, structural, and management scores
- Overall rating
- Geographic location (latitude and longitude)
- Local authority area

The data is loaded into MongoDB from a JSON file and queried directly using PyMongo.

---

## Technologies Used
- **Python**
- **MongoDB**
- **PyMongo**
- **Pandas**
- **Jupyter Notebook**

Key libraries:
- `pymongo`
- `pandas`
- `json`

---
## Notebook Breakdown

### 1) NoSQL_setup_starter.ipynb
This notebook focuses on **database creation and preparation**:
- Connects to a local MongoDB instance
- Creates a database and collection
- Imports establishment data from a JSON file
- Inserts new documents and updates existing ones
- Converts data types (e.g., ratings and coordinates) for accurate querying
- Removes unnecessary records to clean the dataset

---

### 2) NoSQL_analysis_starter.ipynb
This notebook performs **exploratory analysis using MongoDB queries**, including:
- Finding establishments with specific hygiene scores
- Identifying establishments with high ratings in particular local authorities
- Counting establishments that meet given conditions
- Using **MongoDB aggregation pipelines** to:
  - Group results
  - Sort by inspection scores
  - Limit results to top matches
- Converting query results into Pandas DataFrames for readability

---

## Key Concepts Demonstrated
- NoSQL data modeling with MongoDB
- CRUD operations (Create, Read, Update, Delete)
- Querying nested JSON documents
- Aggregation pipelines for analytical queries
- Integrating MongoDB results with Pandas
