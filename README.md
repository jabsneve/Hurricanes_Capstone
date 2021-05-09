![Image of hurricane from ISS](https://www.insurancejournal.com/app/uploads/2018/09/hurricane-768x512.jpg)

# Hurricane Severity Index and Prediction Model

Since 1973 the Saffir-Simpson Hurricane Wind Scale, better known as the Saffir-Simpson Scale, has been the most widely used classification method for tropical cyclones in the Western Hemisphere aka hurricanes. While this scale does serve the purpose of classifying hurricanes based on wind speed it doesn’t address a few important features of tropical cyclones. 

First, the scale is only able to be used for rating hurricanes – storms with maximum sustained winds of at least 64 knots (74 mph). This leaves out any rating of tropical cyclones such as tropical depressions and tropical storms, whom while having lower sustained winds can still generate destructive force on coastal areas.

The other feature not captured by the Saffir-Simpson scale is the size of the storm. This can be measured by the diameter of the storm’s wind field. Simple logic tells us that the larger the area covered by hurricane force winds the larger the area of devastation. 

In 2006 Chris Hebert and Bob Weinzapfel released a new method for measuring tropical cyclone severity named the Hurricane Severity Index (HSI). This index considers both wind speed and wind field size in order to provide a scale more representative of the destructive nature of tropical cyclones. What I have done in this project is utilize data in order to re-create the index then create multiple machine learning models that can be used to predict hurricane category and severity based on storm features.

### Data

NOAA's National Hurricane Center maintains datasets of historical tropical cyclones. The dataset I used for this project is the revised hurricane database, HURDAT2, which includes observations taken from each storm in the Atlantic basin from 1851 to 2019. Wind field radii were not tracked previous to 2004 therefore data from 2003 and earlier were not used for this project. 

* [HURDAT format](https://www.nhc.noaa.gov/data/hurdat/hurdat2-format-nov2019.pdf)
* [HURDAT2 Data (txt)](https://www.nhc.noaa.gov/data/hurdat/hurdat2-1851-2019-052520.txt)
* [Saffir-Simpson Hurricane Wind Scale](https://www.nhc.noaa.gov/aboutsshws.php)
* [Hurricane Severity Index: A More Efficient Way of Predicting a Tropical Cyclone's Destructive Potential](https://ams.confex.com/ams/29Hurricanes/techprogram/paper_168529.htm)

### Data Cleaning

After converting the text data from the HURDAT2 dataset to a csv file I uploaded the data into my Hurricanes notebook for cleaning and processing. The information was fairly orderly with a few issues needing to be addressed – which included:

* Inconsistencies in storm names
* Inconsistencies in dates
* Erroneous time measurements
  * The NHC's official measurements were recorded in 6 hour intervals (0000, 0600, 1200, 1800)
  * Many observations taken at inconsistent times outside of the proper intervals produced erroneous data which had to be removed
* Cyclones with maximum sustained winds of less than 30 knots are not included in the HSI and were removed from the dataset

### EDA & Feature Engineering



### Machine Learning



### Conclusion



### Future Improvement
