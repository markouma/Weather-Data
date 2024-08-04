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

## Q5. What is the mean visibility of the dataset?
The code to solve this is as follows
**df.Visibility_km.mean()**
Mean visibility is **27.664446721311478**
See below

![image](https://github.com/user-attachments/assets/7daa521d-7939-4831-a437-a51679f0144c)

## Q6. Find the number of records where the wind speed is greater than 24 km/hr and visibility is equal to 25 km.
The code to solve this is as follows
**df[(df['Wind Speed_km/h']>24)&(df['Visibility_km']==25)]**
Number of records where the wind speed is greater than 24 km/hr and visibility is equal to 25 km is as below screenshot

![image](https://github.com/user-attachments/assets/0716f09f-daaf-4826-a6ee-89fea0563009)

## Q7. What is the mean value of each column for each weather condition?
I didn't manage to get thye proper solution for this question as all my answers returned errors. The below is the code I use as per my understanding
**df.groupby('Weather_Condition').mean()**
See screenshot below

![image](https://github.com/user-attachments/assets/fe16940f-b826-4616-b0f8-57dab7e6bfa0)

**N/B** I would really appreciate your feedback on this.

## Q8. Find all instances where the weather is clear and the relative humidity is greater than 50, or visibility is above 40.
Code used
**df[(df['Weather_Condition']=='clear') & (df['Rel Hum_%']>50)|(df['Visibility_km']>40)]**

See screenshot below

![image](https://github.com/user-attachments/assets/efc38ed1-c39c-40b5-bebf-ac5aa933ebbc)

## Q9. Find the number of weather conditions that include snow.
Code used
**df[df['Weather_Condition']=='Snow']**
See screenshot below

![image](https://github.com/user-attachments/assets/36dac0ff-a313-41a0-b8fd-6339752db23b)
