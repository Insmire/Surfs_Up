## Overview

The purpose of this project is to pitch the business idea to potential investor W. Avy of setting up a shop named Surf n' Shake in Oahu that will provide surfing equipment and ice cream. For this end, database SQLite table Measurement is queried using object-relational mapper SQLAlchemy. The Measurement table contains temperature observations from January 1, 2010 through August 23, 2017. By W. Avy's request data is filtered specifically for the months of June and December. A summary statistics for each month is then presented as a Pandas DataFrame within Jupyter Notebook SurfsUp_Challenge.ipynb.

---

## Resources

Data source:

    hawaii.sqlite

<!-- "pip show <software>" in command prompt to see pip install ver -->
<!-- pip show code from https://stackoverflow.com/questions/10214827/find-which-version-of-package-is-installed-with-pip -->
Software:

    Jupyter 1.0.0 notebook 6.4.6,
    Pandas
    Python 3.9.7,
    SQLAlchemy 1.4.27, 
    SQLiteStudio 3.3.3,
    Visual Studio Code (VSCode) 1.63.2, 

---

<!-- Results: Provide a bulleted list with three major points from the two analysis deliverables. Use images as support where needed. -->
## Results

### June 2010 - 2017 summary statistics

- A total of 1700 observations are collected.
- The average temperature of June is approximate 75 degrees Fahrenheit.
- The standard deviation is approximate 3 degrees Fahrenheit.
- The minimum temperature is approximate 64 degrees Fahrenheit.
- The maximum temperature is approximate 85 degrees Fahrenheit.

June summary statistics image

![june_temp](https://user-images.githubusercontent.com/96349090/157562847-a126e1ac-da4a-49dd-9ffe-dd26bb04a7d7.png)

### December 2010 - 2016 summary statistics

- A total of 1517 observations are collected.
- The average temperature of December is approximate 71 degrees Fahrenheit.
- The standard deviation is approximate 4 degrees Fahrenheit.
- The minimum temperature is approximate 56 degrees Fahrenheit.
- The maximum temperature is approximate 83 degrees Fahrenheit.

December summary statistics image

![dec_temp](https://user-images.githubusercontent.com/96349090/157562872-573debdc-656b-475b-b245-c154c76975cb.png)

---

<!-- Summary: Provide a high-level summary of the results and two additional queries that you would perform to gather more weather data for June and December. -->
## Summary

Based on the summary statistics, June and December average temperatures, standard deviations, minimum temperatures, and maximum temperatures are fairly similar. The low standard deviations implies temperature variation throughout the years is low during these months. Note that data for June is collected over eight years while the data for December is collected over seven years, resulting in a difference of 183 observations. Summary statistics would be more representative should data for December 2017 also be included in the Measurement table.

In addition to the above summary statistics, a query that a potential investor may also be interested in is the precipitation levels for each month of the year. Should there be a rain season that would affect the number of clients to the shop, the business may benefit from opening only partially each year.

Another query that may be of interest is the number of observations per measurement station. Assuming the stations are evenly distributed within the designated area in Oahu, the temperature and precipitation level observations would be more representative if each station conducted similar observation amounts.
