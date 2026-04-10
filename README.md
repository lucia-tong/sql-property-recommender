# SQL Property Recommender

An accommodation recommendation system built with SQL and Python. Based on real-world client requirements, this project involves constructing a relational database and executing progressive queries to identify properties that meet a specific set of complex filters.
Developed as part of the Master’s in Data & AI — Nuclio Digital School.

## Key Features  

* ETL Process: Converts Excel source files to CSV and loads them into a MySQL database.
* Relational Schema: Creates and manages 4 interconnected tables: Accommodation, Location, Price, and Rating.
* Modular Queries: Develops individual SQL queries for each specific client requirement.
* Advanced Filtering: Combines all constraints into a final query using complex JOINs to return only the properties that satisfy all conditions simultaneously.

## Client Requirements

* Amenities: Must have a terrace and air conditioning; must not have a pool.
* Layout: No studios (must have a separate living room); minimum of 2 bathrooms.
* Size: Minimum surface area of 80m².
* Location: Noise-sensitive client — property must be more than 1 km from the metro and 2 km from the city center.
* Budget: Price per night between €1,500 and €2,000.
* Booking Metric: Reservation percentage must be exactly 25%.
* Ratings: Accommodation score > 4.5 and agency score > 4.

## Project Structure

```
sql-rental-analysis/
├── data/
│   ├── ALOJAMIENTO.csv
│   ├── UBICACION.csv
│   ├── PRECIO.csv
│   └── PUNTUACION.csv
├── sql_queries_analysis.ipynb       # Notebook
└── README.md
```

## Installation & Usage

```bash
pip install sqlalchemy mysql-connector-python pandas openpyxl jupyter
jupyter notebook sql_property_recommender.ipynb
```

Note: A local MySQL instance is required. Update the connection string in the first cell of the notebook with your local credentials.

## Tech Stack

python · pandas · sqlalchemy · mysql · openpyxl · jupyter
