# Data_cleaning_bike
Data Cleaning on London Bike sharing Data
Data Cleaning for London Bike Sharing Dataset

Objective:
The objective of this data cleaning project was to download and manipulate the London bike sharing dataset from Kaggle. The dataset was cleaned and prepared for further analysis and visualization.

Steps Taken:

1. Data Download and Conversion:
   - The dataset, named "London_merged.csv," was downloaded from Kaggle.
   - The downloaded CSV file was converted into a pandas DataFrame for data manipulation and cleaning purposes.

2. Data Inspection:
   - The DataFrame's shape was checked, revealing that it contains 17,414 rows and 10 columns.
   - The data was thoroughly inspected, and it was confirmed that there were no null values in the dataset.

3. Exploring Unique Values:
   - The unique values in the "weather_code" and "season" columns were analyzed.
   - This step helps us understand the different weather conditions and seasons represented in the dataset.

4. Renaming Columns:
   - Some columns in the dataset had inappropriate names.
   - Those columns were renamed with more appropriate and descriptive names to enhance clarity and readability.

5. Normalization of Humidity Column:
   - The "humidity" column contained percentage values.
   - To ensure consistency and compatibility with other numeric values, the percentages were converted into values between 0 and 1.

6. Mapping Actual Values to Weather and Season Columns:
   - The "weather" and "season" columns contained encoded numeric values that were not immediately interpretable.
   - Using the `map` function, the numeric codes in these columns were replaced with actual descriptive values for better understanding.
   - The mappings used were as follows:
   
   For "season":
   - '0.0': 'Spring'
   - '1.0': 'Summer'
   - '2.0': 'Autumn'
   - '3.0': 'Winter'
   
   For "weather":
   - '1.0': 'Clear'
   - '2.0': 'Scattered Clouds'
   - '3.0': 'Broken Clouds'
   - '4.0': 'Cloudy'
   - '7.0': 'Rain'
   - '10.0': 'Rain with Thunderstorm'
   - '26.0': 'Snowfall'
   
7. Exporting Cleaned DataFrame:
   - After completing the data cleaning process, the cleaned DataFrame was exported to an Excel file for future use and analysis.
   - The Excel file containing the cleaned dataset was made available for download.


