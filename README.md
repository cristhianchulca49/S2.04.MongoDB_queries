# Task S2.04 Mongodb_ queries
---

# 🏙️ NYC Restaurants Collection

This repository contains a **MongoDB-based data modeling exercise** focused on working with a **collection of restaurant objects** in New York City. The goal is to explore **document-oriented data structures, queries, and array handling** in a real-world scenario.

---

## 🚀 Skills & Concepts Learned

By completing this exercise, you will practice and reinforce the following skills:

- Understanding **document structure** in MongoDB  
- Working with **nested objects** (`address`, `location`)  
- Handling **arrays of documents** (`grades`) and querying them  
- Using **dot notation** to filter and project nested fields  
- Applying **comparison operators** (`$gt`, `$lt`, `$ne`) on arrays and numbers  
- Filtering data using **$elemMatch** for arrays  
- Using **regex queries** for string matching (e.g., names starting/ending with a substring)  
- Sorting documents by a field (e.g., `cuisine`)  
- Understanding **geospatial data** (longitude and latitude in `location.coordinates`)  
- Translating real-world requirements into **MongoDB queries**  
- Structuring **find() projections** to return only relevant fields  
- Running MongoDB in a **Docker container** with Docker Compose  

---

## 📘 Project Description

For this exercise, we have a collection of **restaurant objects** in New York City with the following structure:

```json
{
  "restaurant_id": Number,
  "name": String,
  "cuisine": String,
  "borough": String,
  "address": {
    "building": String,
    "street": String,
    "zipcode": String
  },
  "location": {
    "type": String,
    "coordinates": [Number, Number]
  },
  "grades": [
    {
      "date": Date,
      "grade": String,
      "score": Number
    }
  ]
}
```
### 🍽️ Fields Description

- **restaurant_id** – Unique identifier for each restaurant  
- **name** – Name of the restaurant  
- **cuisine** – Type of cuisine served  
- **borough** – NYC borough where the restaurant is located  
- **address** – Embedded document with:  
  - `building` – Building number  
  - `street` – Street name  
  - `zipcode` – Postal code  
- **location** – Embedded document with:  
  - `type` – GeoJSON type (usually "Point")  
  - `coordinates` – Array of [longitude, latitude]  
- **grades** – Array of embedded documents with:  
  - `date` – Date of inspection  
  - `grade` – Letter grade (A, B, C…)  
  - `score` – Numeric score assigned  

---

### 🧪 Tools & Technologies Used

- **MongoDB** – NoSQL document database  
- **MongoDB Compass** – GUI to explore collections and documents  
- **Docker** – Containerization for MongoDB  
- **Docker Compose** – Easy setup for running MongoDB locally  
- **mongosh** – MongoDB shell for queries  
- **Git & GitHub** – Version control and project sharing  

---

  ## 🛠️ Installation
Clone this repository:  
git clone https://github.com/cristhianchulca49/S2.03.mongoDB-estructura

---
### 📦 Project Setup

The project includes:

- A `docker-compose.yml` file to start MongoDB with the `nyc` database  
- Example JSON/JS files for the `restaurants` collection  
- Queries demonstrating:
  - Filtering by nested fields and arrays  
  - Using `$elemMatch` for grades  
  - Regex queries for restaurant names  
  - Sorting and projection  
  - Geospatial filters with coordinates
    
---

## 🤝 Contributions are welcome! 
- Please follow these steps to contribute: 
- Fork the repository Create a new branch: git checkout -b feature/NewFeature 
- Make your changes and commit them: git commit -m 'Add New Feature' 
- Push the changes to your branch: git push origin feature/NewFeature 
- Open a Pull Request

