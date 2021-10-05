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

