# BOOT-CAMP WEEK 1 PROJECT

Hello there, the below is how I solved the Week 1 project questions.

After importing the Weather data csv file into my notebook, I imported pandas and then declared my data-frame as "df" to be able to read the imported csv file as shown on the screenshot below.

![image](https://github.com/user-attachments/assets/73662a4a-e310-46f4-a8de-268bd5ddde06)

## Q1. Find all records where the weather was exactly clear.
The code to solve this is as follows
**df.Weather_Condition.value_counts()**
All records where weather was exactly clear are 1326 as shown in the screenshot below

![image](https://github.com/user-attachments/assets/7f596ad4-d4db-4169-a962-de79b6339332)

## Q2. Find the number of times the wind speed was exactly 4 km/hr.
The code to solve this is as follows
**df[df["Wind Speed_km/h"] ==4]**
The number of times the wind speed was exactly 4 km/hr is as shown below

![image](https://github.com/user-attachments/assets/e1d165d3-c126-44a1-b7b8-1c04d63542f0)

## Q3. Check if there are any NULL values present in the dataset.
The code to solve this is as follows
**df.isnull().sum()**
Checking if there are any NULL values present in the dataset, result is **None** as in the screenshot below

![image](https://github.com/user-attachments/assets/298af7ca-454a-465c-ab6c-7034da637c1d)

## Q4. Rename the column "Weather" to "Weather_Condition."
The code to solve this is as follows
**df.rename(columns={'Weather':'Weather_Condition'},inplace=True)**
See the screenshot below

![image](https://github.com/user-attachments/assets/fd25ac78-794d-44b2-818c-aa631fa45d89)
