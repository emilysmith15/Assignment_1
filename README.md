# Analysis of Citi Bike Data from 2013 to 2026

<small> This repository contains an initial cleaning, concatenating, and analysis of Citi Bike ride data, recorded during June of each year since 2013. It is being prepared in support of a story called "Citi Bike Price Increases Mean Shorter Rides." Required Google Doc on story can be found [here](https://docs.google.com/document/d/1D6aKkMMOIjaAMEQsxTA5I7Cnzosploh4IYMja0gojP8/edit?usp=sharing).

# Data

Stored in <code>/data</code>

This analysis includes 2 types of dataset.

The first is Citi Bike ride data, sourced from Citi Bike's own open data webpage, which can be found [here](https://s3.amazonaws.com/tripdata/index.html). This is most of the raw data in <code>/data</code>. For this analysis, I used the data from June of every year since 2013 (including June 2026). June is regularly one of Citi Bike's busiest months. The data was recorded in two different, but similar ways, with the company moving from one to the other in 2019. See [here](https://citibikenyc.com/system-data) for more information on Citi Bike's ride data. The data has been cleaned so that it matches across all years, dropping and renaming some columns from each. 

The following columns were most relevant to the analysis:
+ "ended_at" and "started_at" (or "starttime" and "stoptime" for 2019 and earlier raw data): Used to calculate each ride's duration in order to find yearly averages.
+ "member_casual" (or "usertype" for 2019 and earlier raw data): Used to analyze the rate of subscription over time.
+ "rideable_type": This is the only column that I kept that is only in the post-2019 data. I used it to analyze changes in e-bike vs. regular bike usage over time.


The second is a dataset made manually using Citi Bike's pricing webpage, which can be found [here](https://citibikenyc.com/pricing), and accessing earlier versions of it using the [Wayback Machine](https://web.archive.org/). This dataset is called <code>/Citi_Bike_Prices.csv</code>.

The following columns were most relevant to the analysis:
+ "Annual Membership" and "Day Pass": Used to analyze price changes over time. 


# Methodology

The notebook <code>/Citibike_June.ipynb</code> contains the cleaning, concatenating and analysis of the data. The following analyses were conducted: 


TK
Tk
TK

# Outputs

There are outputs for each analysis, as noted above. 

# Running the Analysis Yourself

You can run the analysis yourself. To do so, you'll need the following installed on your computer:
+ Python 3

# Licensing 

All code in this repository is available under the [MIT License](https://opensource.org/license/MIT). The data file in the output/ directory is available under the [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/) license. All files in the data/ directory are released into the public domain.

# Feedback / Questions?
Contact Emily Smith at emily.smith15@journalism.cuny.edu.
