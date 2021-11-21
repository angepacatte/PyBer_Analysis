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
