## Climate Analysis and Exploration
To begin, I used Python and SQLAlchemy to do basic climate analysis and data exploration of the climate database. All of the following analysis was completed using SQLAlchemy ORM queries, Pandas, and Matplotlib.

* Used SQLAlchemy `create_engine` to connect to the sqlite database.
* Used SQLAlchemy `automap_base()` to reflect  tables into classes and save a reference to those classes called `Station` and `Measurement`.

### Precipitation Analysis
* Designed a query to retrieve the last 12 months of precipitation data.

* Selected only the `date` and `prcp` values.

* Loaded the query results into a Pandas DataFrame and set the index to the date column.

* Sorted the DataFrame values by `date`.

* Plotted the results using the DataFrame `plot` method.

* Used Pandas to print the summary statistics for the precipitation data.

### Station Analysis
* Designed a query to calculate the total number of stations.

* Designed a query to find the most active stations.

    * Listed the stations and observation counts in descending order.

* Designed a query to retrieve the last 12 months of temperature observation data (tobs).

* Filtered by the station with the highest number of observations.

* Plotted the results as a histogram with `bins=12`.

### Temperature Analysis 

* Used the `calc_temps` function to calculate the min, avg, and max temperatures.

* Plotted the min, avg, and max temperature from your previous query as a bar chart.

* Used the average temperature as the bar height.

* Used the peak-to-peak (tmax-tmin) value as the y error bar (yerr).

