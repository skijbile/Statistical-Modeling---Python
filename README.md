# Final-Project-Statistical-Modelling-with-Python

## Project/Goals
To be able to pull data from API's,understanding first hand its advantages and disadvantages so that I will be familiar with steps that can be taken to avoid any conflicts. Usage of the data appropriately to get the desired result by being able to comfortably parse through json files.
Being able to grasp the steps that would be required to build a model by selecting the correct target variables and grouping the right data

## Process
Step 1 : This part was to pull the data from API's where all three API's were very different from each other and each had different challenges. After multiple attempts on each API, I understood the importance of saving the json file and also pushing the folder to git_hub to avoid loss of data or having issues with cost,rate of limitations that may occur with some api's. For this project I did not go into too much details with pulling  of data with the various different parameters avible but went with the basics of latitude, longitude,radius provided.

Step 2: There was a lot of back and forth within each notebook to make sure that the information is presented correctly in each of the data frames and also making a lat_lon column which would act as a primary_key along with any other column so that each row was a unique value.

You can find all the csv files created and the json files from all the api's in the data folder along with the database created with SQlite

Description of each notebook in order of process available in the notebooks folder:

city_bikes.ipynb - This has the steps to request data from the city bikes api, and pasrse through the json files to get relevant information for the city of choice(Paris).

yelp_foursquare_EDA.ipynb -  This note book contains the process of using the latitude and longitude from the city bikes data and acquiring the related businesses in the area specified and providing a comparison of the the two api's based on the results returned. 

joining_data.ipynb - Here I connected the information from city_bikes and yelp api's and performed some EDA and plotts before creating a model.

model-building.ipynb - In this notebook i perfomed backward selection method to build a regression model and note down the obeservations.


## Results
I chose Paris as my city and I soon realised that my data set was too big as the city I chose was a big one , I limited my data to  the first 500 data points to make it easier to pull data from the other api's. I found that yelp api though limited to only the food and beverage industry gave a lot more data with regards to the business in comparision to the four_sq api which has multiple parameters and categories on which you can get geo-graphical related results in and around the set parameters.

## Challenges 
There were multiple challenges I faced from my jupyter notebook crashing after pulling data the first time which made me implement a different method to pull data and save as it happens to me reaching the limits to yelp request and loosing the data as I misunderstood midnight UTC for just midnight and ran my get request again and ended up re-writing my saved file.
These were all technical challenges but simultaneously parsing through the right data and being able to understand how to know what is important and change it according to the requirements of the project posed as a challenge as it was a lot of back and forth in the notebooks and being able to keep the steps in order of which they need  to be run (to be able to have access to the data right) created a lot of confusion.

## Future Goals
If  i had more time i would have definately liked to pull more data specially from four_sq api, based on some of the different parameters and joined it with the yelp api to give me a more better rounded data and more common data points to create a model. 
