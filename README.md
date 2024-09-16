This project is about doing a climate analysis about the Hawai area. 
we have 2 files in this project, Surfsup and app.py. 

The first part analyzes and explores the climate data. 
We used SQLAlchemy to connect SQLDatabase and an automap function to reflect tables into classes. 
We started by finding the most recent date in the dataset which is "2017-08-23". Moving on, we designed a query to retrieve the last 12 months of precipitation data and plotted the results using Pandas and Matplotlib. 
 <img width="910" alt="Screenshot 2024-09-16 at 8 28 07 AM" src="https://github.com/user-attachments/assets/a60d14ec-b2b8-4163-8eab-a6878085095e">
 We then calculated the summary statistics for that same data and the results will be shown below. 
<img width="198" alt="Screenshot 2024-09-16 at 8 28 58 AM" src="https://github.com/user-attachments/assets/8e3ecfee-c139-4ddb-86a9-400e1f37aa75">
The next part we explodes the station analysis by getting the most attractive stations. 
We calculted the lowest, highest, and average temperature of the most active station id. The lowest temperature is 54.0, the highest is 85.0, and the average is 71.66378066378067. 
We then plotted the results in a histogram for the last 12 months of temperature observation data. 
<img width="668" alt="Screenshot 2024-09-16 at 8 31 14 AM" src="https://github.com/user-attachments/assets/a70a9d07-6c5e-4b67-ba48-c7bac2dd5481">

Moving onto our second file called app.py. We designed a Flask API based on the queries developed. 
1st route: Returns the last 12 months of precipitation data 
2nd route: Returns a JSON list of weather stations from the dataset.
3d route: Returns the dates and temperature observations of the most active station for the previous year of data.
4th route: Returns a JSON list of the minimum temperature (`TMIN`), average temperature (`TAVG'), and maximum temperature (`TMAX`) for the specified date range.


