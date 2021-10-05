# AirBnB-Dataset-Preparation-cleaning

- OpenRefine video link - https://youtu.be/m1u-2IME7g8
- Noisy dataset - https://raw.githubusercontent.com/AnishaA-git/AirBnB-Dataset-Preparation-cleaning/master/AB_NYC_2019.csv
- Cleaned Dataset - https://raw.githubusercontent.com/AnishaA-git/AirBnB-Dataset-Preparation-cleaning/master/AB_NYC_2019_1.csv
- Pandas Profiling - https://github.com/AnishaA-git/AirBnB-Dataset-Preparation-cleaning/blob/master/Pandas%20Profiling%20Report.pdf
- Colab - https://github.com/AnishaA-git/AirBnB-Dataset-Preparation-cleaning/blob/master/HW_1_airbnb_data_analysis.ipynb

# Steps of OpenRefine
The name, host_name, last_review and reviews_per_month columns had missing values.   
The missing values originate from a variety of reasons:
- The host or person inputting data may have forgotten to enter the value.
- Hardware or software error during the collection is affecting accuracy of trip data and so on.

Additionally, it is recommended to make the missing values a required field for listing data collection purposes to avoid missing data in the future.

The majority of the missing data is from the "last_review" and "reviews_per_month" columns. Since the other two columns only had relatively few missing values, thus, deleted the associated rows.
- Removed "host_name" and "name" missing values, as they are not that significant to the dataset and also the number of missing values were very small as compared to "last_review" and "reviews_per_month"
- Filled "reviews_per_month" values as "0" 
- Filled "last_review" values as last date of 2019 year that is "2019-12-31"

# Summary of Data

#### Availability
- There are 48858 listings in total.
- The majority of the listings are Entire home/apts or Private rooms.

- On average, any given listing is available <b>110 days</b> in a year.
    - Listings in <b>Staten Island</b> have the greatest availability and receive the most reviews per listing. 
    - However, Staten Island also receives the least number of reviews overall.
    - Listings in <b>Broklyn</b> have the least availability and receive the second least reviews per listing. 
    - However, Broklyn receives the highest number of reviews overall.
    
- Average duration of stay for all listings is 7 days.
    - Listings in the <b>Spuyten Duyvil</b> neighbourhood offer the longest average duration of stay at approximately <b>48 days.</b>
    - Listings in the <b>Manhattan</b> neighbourhood group offer the longest average duration of stay at approximately <b>8 days.</b>

#### Price 

- Average Price Across all listings: 142.77
- There are <b>60</b> neighbourhoods with average listing price above the average for all listings.
- There are <b>161</b> neighbourhoods with average listing price below the average for all listings.
- Largest standard deviation in price is in <b>Manhattan</b>.
- The spread of prices is greatest in <b>Manhattan.</b>
- As expected, listings with Entire home/apt are the most expensive.

#### Number of Reviews

- Across all categories (Room Type, Neighbourhood etc.), less expensive Listings receive more reviews. 
- The majority of reviews are left in the month of <b>June</b> which indicates that the majority of customers used a rental in June. Meanwhile, the least reviews are left in <b>February</b>, which indicates that the  fewest customers used a rental in February.
- Staten Island has the largest number of reviews as compared to the actual number of listings, which indicates that reviews were left more frequently for stays in listings that were within the Staten island neighbourhood group.
- Manhattan has the second largest number of listings but has the least number of reviews compared to the actual number of listings, which indicates that reviews are left less frequently for stays in the Manhattan neighbourhood group. The possible reasons for this are as follows:

    - The average listing price is also the highest of all neighbourhood groups.
    - Manhattan's average listing price is also above the average for all listings.
