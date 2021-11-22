                            #**PyBer Analysis Written Report**


##*Overview of the Analysis*
  
  The purpose of this analysis was to look at PyBer ride sharing services in different types of cities and compare a few variables.  The types were broken into 3 categories of urban, suburban, and rural.  Two dataframe, city_data_df and ride_data_df were merged together so all information was in one place.  The image below shows the pyber_data_df which was the dataframe created from the two original dataframes.
  
 
 <img width="724" alt="Screen Shot 2021-11-21 at 9 26 41 AM" src="https://user-images.githubusercontent.com/85581208/142768151-a7279bfb-c236-411f-aae7-7c2fc1897c5c.png">
  
  
  The variables calculated for the analysis included total_ride_count_by_type, total_driver_by_type, total_fares_by_type, avg_fare_per_ride_by_type, and avg_fare_per_type_per_driver. The groupby function with either the sum or mean function was utilized to calculate the variables abover. The merged dataframe was referenced for all  except for total_driver_by_type the city_data_df was used so that there was not overlapping in summing of the total drivers by city type.  The image below shows the code used.

<img width="521" alt="Screen Shot 2021-11-21 at 9 33 54 AM" src="https://user-images.githubusercontent.com/85581208/142768409-9774b00a-b83c-40ed-b7b8-9bbea955348c.png">

With these new values a pyber_summary_df was created.  The data was summed up nicely and gave a nice comparison of the different areas of ride sharing per city type.  The picture below shows the dictionary created to form the summary dataframe.

<img width="508" alt="Screen Shot 2021-11-21 at 9 37 48 AM" src="https://user-images.githubusercontent.com/85581208/142768553-acff3a0b-313d-456b-9170-1dadda0f8e42.png">

The columns were then formatted with the final view of the pyber_summary_df appearing as shown in the next image.

<img width="397" alt="Screen Shot 2021-11-21 at 9 41 43 AM" src="https://user-images.githubusercontent.com/85581208/142768692-68662727-6bf8-4f74-9ef5-66f581666737.png">

  The final part of the analysis included using the groupby function to group into type, date and summing up the fares.  This spinoff dataframe was then used to create a pivot table.  The pivot table was created as seen in the image inserted below.  This basically allowed for more analysis by date using the 'loc' function.


<img width="721" alt="Screen Shot 2021-11-21 at 9 45 56 AM" src="https://user-images.githubusercontent.com/85581208/142768855-470c064e-7ae2-44ee-a25d-f84a92d39158.png">


The pivot table broke the fares by city type down the dates January through April.  Allowing for a look at seasonal trends in fares.


##*Analysis Results*
  The first part of the analysis demonstrated there is a big difference in volume between urban, suburban, and rural cities.  Rural cities only had 125 rides compared to 625 for suburban and 1,625 for urban.  The proportion of drivers per total rides differed greatly per city type as well.  The urban cities has 2,405 drivers while the rural only had 78 drivers.  Less drivers than total rides in rural areas.  The suburban areas have a total of 490 drivers.  The amount of drivers per city type may have to do with more overnight drivers needed in the more populated areas where in the rural areas things shut down earlier in the evening.
  
  Total fares for the city types were as follows -  urban was $39,854.38, suburban was $19,356.33, and rural was $4,327.93.  Rural cities averaged a higher fare per ride at $34.62.  Suburban was right in the middle averaging $30.97 a ride.  Urban rides averaged $24.53 a ride which is around $10 less than the rural average.
  
  The last mearurement was the average fare per driver.  There was a big difference between rural and urban.  Rural was was almost $40 per driver at $55.49 while the urban averag fare per driver was $16.57.  The suburan average was in the middle at $39.50.
  
  The last analysis looking at times was converted into a line chart with a line for each city type.  The line chart below gives a good visualization of fares during the months of January through April.
  
  ![Total Fare by City Type](https://user-images.githubusercontent.com/85581208/142781338-c61454a6-1b32-440d-bfc8-fa045ce4f847.png)
  
 
 Overall none of the lines cross.  The total of the fares stay in their own range per city type. Urban fares were always higher no matter what month.  Surburban fares in the middle and rural with the cheapest fares. The end of February appears to have a peak in the total fares for all 3 city types.  Urban fares were the lowest in the beginning of Janurary.  Suburban total fares had a the lowest total in the beginning of January, beginning of March, and mid-April.  The rural total fares had less fluctuation with a dip in January and the middle of February.
 
 ##*Analysis Summary*
  After finishing the analysis, there are a few recommendations that can be made.  January should be targeted in all 3 city types.  Fare totals were some of the lowest across the board.  The suburban and urban totals increased as January went on but the rural cities total fare did not.  Possibly lowering fares or a marketing plan may help increase the fare totals.  
  Another area to focus are the number of drivers in urban areas.  There are many more than actual drive count.  Either drivers are not making themselves visible enough on the app or maybe there are too many drivers in the urban area.  
  More analysis could be done on the fares being charged in high traffic times.  When demand is up, are fares being increased to make more of a profit when people are more willing to pay whatever is charged. Also it would be good to explore if some drivers are willing to cover other city types.  For instance, urban drivers cover the rural cities when demand is not being met.
 
