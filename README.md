# PyBer_Analysis
# Overview of the analysis: 

## Looking into fare disparity
In our initial analysis of PyBer rideshare data we found that the average rural ride fare is significantly more than in urban cities, about $5 more per ride. V. Isualize tasked us with a new analysis to summarize the data by city type to hopefully uncover possible reasons for the large disparity between city type fares and make a recommendation to the CEO to address it. 

# Results:

## Distinct community sizes
After we merged the city and ride csvs into one dataframe we used the groupby method to summarize the number of rides, drivers, and fares for each city type. The result showed significant differences in total rides, drivers, and fares based on city type. 

Here are screenshots of the findings:
## Rides
<img width="806" alt="Ride_count" src="https://user-images.githubusercontent.com/66224990/168481242-556868f2-59c3-4b14-8463-819ee399e8e3.png">

## Drivers
<img width="845" alt="Driver_count" src="https://user-images.githubusercontent.com/66224990/168481277-64eb7d6f-1099-435a-a549-c159e1c58a79.png">

## Fares
<img width="745" alt="Fare_total" src="https://user-images.githubusercontent.com/66224990/168481343-47dc786e-2911-4585-8221-c0a95df25c3f.png">

## Average per ride and driver
<img width="783" alt="Avg_fares" src="https://user-images.githubusercontent.com/66224990/168482072-8153c14f-4b82-445c-9648-54230fa9b4b8.png">

While there are around 30 times more urban drivers in the PyBer pool than rural areas, the difference in total fares was only about 9 times more. This results in the average fare for each ride and driver is significantly less in urban areas than in rural ones.

We then plotted the total fares by city type into a line graph, below. 

![PyBer_fare_summary](https://user-images.githubusercontent.com/66224990/168478691-0d4f0d23-935c-4d76-9386-bbb182e7e59a.png)

The line graph illustrates the total fares by city type. Given the great difference in the number of drivers between urban, suburban, and rural communities it is not surprising that they would have the largest to smallest total fares in that order. Interestingly we saw they all follow a simialar trend throughout the 4 months we analyzed with various peaks and declines. They all also showed a steep decline in May.

# Summary: 

## Why the large disparity in rural and urban fares?

If drivers are able to set their own rates for each ride then it would make sense that urban areas would be able to keep their fare per ride lower than in rural areas. A larger population of drivers would create more competition and demand to keep prices low. They also would have a higher volume of rideshare clients than rural areas so they can charge less per ride. Another reason for urban drivers charging less per ride is that urban areas typically have more job opportunities than rural ones so the urban PyBer drivers are more likely to offer rides as a secondary job. 

## Our Recommendations

We can recommend additional analysis to help the CEO address the disparities among the city type ride share fates. If we could analyze the following data points it may shed more light on why there is a disparity between the fares. 

* Time of day: The data we were provided included the time of day that the ride was provided. Rural and urban lifestyles may differ and affect when people are requesting rides. The driver may adjust their rates depending what time of day the driver is accepting the gig.  
* Ride distance and time: The data sets we were given did not include the distance of each ride, but it is likely that rural rides have to cover more distance than urban ones per ride. This would result in each ride taking more time for the driver to complete each ride gig. 
* Amentities & car type: Some rideshare drivers offer amenities to their clients like snacks and beverages. Some drivers may have more luxury vehicles than others. If we had data for amenities and car type it may point to another reason why drivers in certain areas are charging more per ride.

If the CEO is concerned about removing the disparity between rideshare fares they would need to implement a standard ride fare and not allow drivers to set their own rates. However, removing the ability for drivers to set their rates would give them less incentive to provide the best service or any amenities. It may also result in drivers in suburban and rural areas leaving because the prices would be lowered to a level that is not monetarily viable due to the smaller volume of clientele in those areas. 
