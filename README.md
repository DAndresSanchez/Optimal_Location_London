# Optimal location for studying in London
## Capstone Project
### IBM Data Science Professional Certificate
https://www.coursera.org/learn/applied-data-science-capstone


#### Business problem description

Which is the most recommended location for living in London assuming you want to study at Middlesex University? The accommodation needs to be close to the university, but not too far from the city centre. Supermarkets and cafes in the neighborhood will also be taken into consideration. However, being a student the rent is a key factor to bear in mind. A one bedroom house or flat is preferred. 

London is a large city with plenty of opportunities. There are many interesting spots in this city, touristic attractions, monuments and even business areas. All these factors are important for looking for accommodation. Rental prices in London are high, the area must be chosen in a way that minimises it while still enjoying the proximity to the key locations mentioned before.

The target audience is university students who are looking for accommodation in London, and don't want to give up on all the beauties of London. 


#### Data

The different boroughs of London will be checked, searching for venues of interest and average rental prices.

Data sources:
- Foursquare
- https://data.london.gov.uk/dataset/average-private-rents-borough
- https://data.london.gov.uk/dataset/postcode-directory-for-london
- https://www.freemaptools.com/download/outcode-postcodes/postcode-outcodes.csv
- https://www.doogal.co.uk/PostcodeDistrictsCSV.ashx

The accomodation must be located close to Middlesex University. Foursquare data will be used to search for venues around this location. The postcode directory of the city will be used to group the venues information and average rent per area by borough.


![Clustering](/images/London_locations.png)


### Results
In order to make a more conclusive analysis, more variables should be taken into consideration. For example, take-away venues may be of importance to the user, or small food stores. However, for the sake of simplicity only cafes and supermarkets have been considered in this study. Also, the distance to the closest metro station would be relevant to be added, since it is key in a city like London.

In general the results make sense and are as expected.


### Discussion
- Label 0 (blue): lowest rent, but far from university and city centre. Also a medium number of cafes and shops.
- Label 1 (yellow): second lowest rent, shortest distance to university and short distance to city centre. No supermarkets in the area and very low number of cafes. 
- Label 2 (green): affordable rents, medium distance to university and city centre. Good number of cafes and supermarkets.
- Label 3 (red): expensive area, medium distance to university but close to city centre. A great number of cafes and medium number of supermarkets.
- Label 4 (orange): very expensive area, located in city centre, medium distance to university. A medium number of cafes and medium-low number of supermarkets.
- Label 5 (purple): cheap rents, far from both university and city centre. No cafes or shops.


### Conclusion
The final choice has to be made by the person who is going to live and study in London. However, based on the analysis, __the most suitable location would be either regions in yellow (1) or in blue (green)__, depending on the preference of the user. If the main priority is being close to university, then the user should choose the yellow regions (1). If on the contrary the number of cafes and supermarkets is relevant, the user should go for the green regions (2). This conclusion is assuming the rent is a key factor to take into account due to the student condition.