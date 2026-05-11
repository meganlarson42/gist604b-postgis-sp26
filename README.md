# PostGIS Database Orchestration

**Student:** Megan Larson

**Course:** GIST 604B – Open Source GIS

**Module:** Module 4 - PostGIS Database Orchestration

**University of Arizona**

## Project Description
This project involved setting up a professional spatial database environment to analyze New York City geographic data. I learned how to store map shapes in a database and write SQL queries to answer complex spatial questions about neighborhoods, streets, and subway stations.

## Tools and Technologies
- PostgreSQL & PostGIS (Spatial Database)
- Docker & Docker Compose (Containerization)
- SQL (Structured Query Language)
- GitHub Codespaces
- shp2pgsql (Data Import Tool)

## What I Did
- **Built a Database Environment:** Used Docker to launch a PostGIS-enabled database and connected it to VS Code to manage spatial tables.
- **Imported Map Data:** Converted standard shapefiles (neighborhoods, census blocks, streets, and subways) into database tables using the shp2pgsql command-line tool.
- **Wrote Spatial Queries:** Created SQL scripts to perform basic data searches and advanced geometry calculations, such as finding distances and areas.
- **Analyzed Spatial Relationships:** Used SQL to determine how different map layers interact, such as checking which subway stations fall within specific neighborhoods.
- **Performed Spatial Joins:** Combined data from multiple tables based on their physical location to create new insights into NYC's urban infrastructure.

## How to View / Run
- **Start Database:** Run docker compose up -d in the terminal to start the PostGIS container.
- **Connect:** Use the PostgreSQL Explorer in VS Code with the username and password postgres to view the nyc database.
- **Execute Queries:** Open the files in the sql/ folder, highlight a query, right-click, and select Run Query to see the results.

## Repository Structure

    .
    ├── README.md
    ├── .devcontainer
    │   ├── devcontainer.json
    │   └── Dockerfile
    ├── sql/
    │   ├── 01_basic_sql_queries.sql
    │   ├── 02_geometry_queries.sql
    │   ├── 03_spatial_relationships.sql
    │   └── 04_spatial_joins.sql
    ├── demos/
    │   ├── demo_aggregation_queries.sql
    │   ├── demo_basic_queries.sql
    │   ├── demo_filtering_queries.sql
    │   └── demo_postgis_queries.sql
    └── docker-compose.yml

## Notes

- demos folder contains sql scripts discussed in the lectures.
- SQL files contain exercises and hints.
- Write and execute queries directly in the `sql/` files using the VS Code PostgreSQL extension.
- Data is downloaded and prepared inside the Codespace environment and is not stored in this repository.
- The database runs in a separate PostGIS container using Docker.
