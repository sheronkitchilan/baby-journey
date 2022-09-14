# Introduction

Case study for Airbnb listing data for the city of Amsterdam

Airbnb is a paid community platform for renting and booking private accommodation founded in 2008. Airbnb allows individuals to rent all or part of their own home as extra accommodation. The site offers a search and booking platform between the person offering their accommodation and the vacationer who wishes to rent it. It covers more than 1.5 million advertisements in more than 34,000 cities and 191 countries. 

The given data set size 6173 records and 18 columns

### Data Dictionary
- id - Airbnb's unique identifier for the listing                                  
- name - Name of the listing                              
- host_id - Airbnb's unique identifier for the host/user                             
- host_name - Name of the host. Usually just the first name(s).                         
- neighbourhood_group - The neighbourhood group as geocoded using the latitude and longitude against neighborhoods as defined by open or public digital shapefiles.  
- neighbourhood- The neighbourhood as geocoded using the latitude and longitude against neighborhoods as defined by open or public digital shapefiles.  
- latitude- Uses the World Geodetic System (WGS84) projection for latitude and longitude.                         
- longitude- Uses the World Geodetic System (WGS84) projection for latitude and longitude.                        
- room_type - "[Entire home/apt|Private room|Shared room|Hotel]

All homes are grouped into the following three room types:

Entire place
Private room
Shared room
Entire place
Entire places are best if you're seeking a home away from home. With an entire place, you'll have the whole space to yourself. This usually includes a bedroom, a bathroom, a kitchen, and a separate, dedicated entrance. Hosts should note in the description if they'll be on the property or not (ex: ""Host occupies first floor of the home""), and provide further details on the listing.

Private rooms
Private rooms are great for when you prefer a little privacy, and still value a local connection. When you book a private room, you'll have your own private room for sleeping and may share some spaces with others. You might need to walk through indoor spaces that another host or guest may occupy to get to your room.

Shared rooms
Shared rooms are for when you don't mind sharing a space with others. When you book a shared room, you'll be sleeping in a space that is shared with others and share the entire space with other people. Shared rooms are popular among flexible travelers looking for new friends and budget-friendly stays."                        
- price - Daily price in local currency                            
- minimum_nights  - Minimum number of night stay for the listing (calendar rules may be different)                  
- number_of_reviews  - The number of reviews the listing has               
- last_review    - The date of the last/newest review                    
- reviews_per_month  - The number of reviews the listing has over the lifetime of the listing           
- calculated_host_listings_count  - The number of listings the host has in the current scrape, in the city/region geography.   
- availability_365    - avaliability_365. The availability of the listing 365 days in the future as determined by the calendar. Note a listing may not be available because it has been booked by a guest or blocked by the host.               
- number_of_reviews_ltm  - The number of reviews the listing has (in the last 12 months)            
- license  - The licence/permit/registration number                     

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

