# sqlalchemy-challenge

# Climate Analysis and Flask API

This project involves analyzing climate data from the island of Hawaii and creating a Flask API to provide access to the data through various routes.

## Dataset

The dataset used for the analysis is stored in a SQLite database file named "hawaii.sqlite" located in the "Resources" folder. It contains two tables: "Measurement" and "Station".

## Jupyter Notebook Code

The code in the Jupyter Notebook file "climate_starter.ipynb" performs the following tasks:

1. Importing the necessary dependencies and setting up the database connection.

2. Retrieving the most recent date in the dataset and calculating the date one year prior to that.

3. Querying the precipitation data for the last 12 months and plotting it as a line graph.

4. Calculating the summary statistics for the precipitation data.

5. Finding the total number of stations in the dataset.

6. Determining the most active stations and their row counts in descending order.

7. Calculating the lowest, highest, and average temperature for the most active station.

8. Querying the temperature observations for the last 12 months of the most active station and plotting it as a histogram.

9. Closing the database session.

## Flask API

The Flask API is implemented in the "app.py" file and provides the following routes:

1. `/` (Homepage): Displays a welcome message and lists all available API routes.

2. `/api/v1.0/precipitation`: Retrieves the last 12 months of precipitation data and returns it as a JSON object with date as the key and prcp as the value.

3. `/api/v1.0/stations`: Retrieves the list of stations from the dataset and returns it as a JSON list.

4. `/api/v1.0/tobs`: Retrieves the temperature observations for the last 12 months of the most active station and returns them as a JSON list.

5. `/api/v1.0/<start>`: Calculates the minimum, maximum, and average temperature for all dates greater than or equal to the specified start date and returns them as a JSON object.

6. `/api/v1.0/<start>/<end>`: Calculates the minimum, maximum, and average temperature for the specified date range (inclusive) and returns them as a JSON object.

# Refrences
https://github.com/Baylex/surfs_up/blob/main
https://flask.palletsprojects.com/
https://docs.sqlalchemy.org/
https://www.sqlite.org/docs.html

