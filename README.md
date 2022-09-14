# Introduction

Case study for Airbnb listing data for the city of Amsterdam

Airbnb is a paid community platform for renting and booking private accommodation founded in 2008. Airbnb allows individuals to rent all or part of their own home as extra accommodation. The site offers a search and booking platform between the person offering their accommodation and the vacationer who wishes to rent it. It covers more than 1.5 million advertisements in more than 34,000 cities and 191 countries. 

The given data set size 6173 records and 18 columns

### Data Dictionary
- id - Airbnb's unique identifier for the listing                                  
- name - Name of the listing                              
- host_id - Airbnb's unique identifier for the host/user                             
- host_name - Name of the host. Usually just the first name(s).                         
- neighbourhood_group - The neighbourhood group as geocoded using the latitude and longitude against neighborhoods as defined by open or public digital shapefiles.  - neighbourhood - The neighbourhood as geocoded using the latitude and longitude against neighborhoods as defined by open or public digital shapefiles.             - latitude - Uses the World Geodetic System (WGS84) projection for latitude and longitude.                         
- longitude - Uses the World Geodetic System (WGS84) projection for latitude and longitude.                        
- room_type                         
- price                             
- minimum_nights                    
- number_of_reviews                 
- last_review                        
- reviews_per_month                 
- calculated_host_listings_count     
- availability_365                   
- number_of_reviews_ltm              
- license                       

## Content

- Importing libraries
- Load dataset
- Check for missing values
- Data pre-processing
  - Check for duplicates
  - Drop unnecessary columns
- Data Visualization
- Regression Model
- Conclusion

### Conclusion

Data analysis was conducted on the given dataset after performing proper data cleansing tasks and interpritaions were given to each visualization.

It is evident that majority of the room type which is accessed by people are Entire Home/apt and private room over hotel rooms and shared rooms. Price range of entire home/apt varies around 100-300 euro per night and private room varies around 50-150 euro per night. Most popular neighbourhood can be listed as De Baarsjes -Oud West and Centrum- West. The numbers go hand in hand for the given neighbourhood when compared to rest of the list. When comparing availability-365 variable over lattitude and longitude it is evident that majority of the prpoperties were not avilable through out the year. Reviews per month and number of reviews show a relatively higher correlation (64%) reviews per month and number of reviews ltm are highly correalted. (88%) Finally, performed a linear regression analysis with 7 independent and price as the dependent variable and received R squared value around 11%, which clearly mentions that included independent variables are not explainng the dependent variable price, hence we need to improvise the data model by increaing the data size by performing Feature engineering to include more signifant variables into the model.

