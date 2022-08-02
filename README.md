# Airline-Delay-Analysis
This is a capstone project from #30Daysoflearning hosted by Theoyinbooke. The project is aimed at telling a flight experience story.
For this project, I want to understand what causes flight delay and how it can be reduced.
Delayed flight reduces customers satisfaction and it also comes at a cost to the airport.

## About data
The dataset is made on Oyinbooke Github Repository for the purpose of this analysis. You can a [view here](https://github.com/theoyinbooke/30Days-of-Learning-Data-Analysis-Using-Power-BI-for-Students/blob/main/Airline%20Project/Airlines.csv).

### Problem statement
This analysis answers the following questions:
1)  What has been the history of flight experiences in the past?
2) How bad was delayed flights?
3) Any identified pattern with delayed flights?
4) Causes of airplane delay?

### Data Transformation
I had to change the data types of some selected columns.

![image](https://user-images.githubusercontent.com/104326012/182299964-6584c903-93af-454b-aeae-92ff90e976e9.png)

I changed the delay column to TRUE or FALSE

I added conditional column to Days of thr week column.

![image](https://user-images.githubusercontent.com/104326012/182299866-524b33e3-f6e5-4a74-8b47-8ba5d23cb094.png)

I imported another dataset from BTS.gov detailing the cause of airline delays over the years and this was useful for our analysis, I had to clean the dataset and removed unuseful columns.

![image](https://user-images.githubusercontent.com/104326012/182301006-414f8ecb-c4c3-4389-bef5-f1f8bae2b2c7.png)

I replaced all NULLS with 0

![image](https://user-images.githubusercontent.com/104326012/182301180-b5ec2918-b995-43af-96b5-b55489c90f20.png)

## Analysis
I created 4 Dax measures;

![image](https://user-images.githubusercontent.com/104326012/182301900-6f0a2ed9-667a-409f-8e56-462c07431662.png)
    
    Average of the total delayed time 

![image](https://user-images.githubusercontent.com/104326012/182301939-ba1e3a8b-0e0a-49ea-be7d-0c61ff0774ba.png)
    
    Count the number of rows that are delayed

![image](https://user-images.githubusercontent.com/104326012/182301988-0df674b2-9ef1-4961-9a4b-2c1b7828341f.png)
    
    Count the number of rows that are not delayed

![image](https://user-images.githubusercontent.com/104326012/182302068-d1c7136c-f968-44ad-a851-ffc581983991.png)
    
    Ratio of the delayed time to on-time flights in percentage rounded up to 2 d.p
    
Now its time to tell our story!

It is important to note that a larger percentage of our flights were on-time(55.46%) and 44.54% were delayed. However, we are only interested in the delayed flights - the cause and how bad did they delayed.

1)  What has been the history of flight experiences in the past?

![image](https://user-images.githubusercontent.com/104326012/182303504-bf38451e-aed7-4aae-a2a9-23dc80adbc4f.png)

2) How bad was delayed flights?

![image](https://user-images.githubusercontent.com/104326012/182304407-87976af1-ffc0-44bc-9c6e-9d82daacb196.png)
![image](https://user-images.githubusercontent.com/104326012/182304507-58d8d947-3230-41e8-b93c-5d3c4537d6b2.png)


    FL airline delayed the most with an average of about 928 minutes. 

3) Any identified pattern with delayed flights?

![image](https://user-images.githubusercontent.com/104326012/182304695-85728e13-fdcd-4dee-9342-05b6f1aebf5e.png)

   Most flights experienced delays on weekdays due to influx of customers 

4) Causes of airplane delay?

![image](https://user-images.githubusercontent.com/104326012/182305057-1620f07c-dd28-4865-ac81-65269d7247ef.png)

    Most of the delay is due to the arrival of the same airline from another airport.
    
    
  ## Recommendations
  1) Airlines should be given at least 1hour time interval between their arrival time and their next flights.
  2) Airlines with lower delays should be booked.
  3) More flights should be scheduled on weekends to reduce delay.
