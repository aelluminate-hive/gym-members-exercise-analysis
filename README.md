# Gym Members Exercise Analysis

This project explores the analysis of a fitness dataset that includes various features such as age, gender, weight, height, heart rate metrics, workout sessions, and fitness habits. The dataset, consisting of 973 records, is loaded and examined through exploratory data analysis (EDA) to uncover insights about exercise patterns, calorie consumption, body composition, and overall fitness levels. A custom function groups the dataset by age ranges to analyze trends across demographics.

The analysis reveals key statistics such as average age, body mass index (BMI), workout duration, and calories burned. Additionally, the data highlights correlations between workout type, frequency, and physiological markers like heart rate and fat percentage. Through this project, we aim to provide a comprehensive understanding of fitness behaviors and factors that influence exercise outcomes, contributing to improved fitness planning and health management.

## Objectives 

1. **Data Exploration**: Load and examine the dataset to understand its structure and contents.
2. **Descriptive Statistics**: Calculate key statistics such as average age, BMI, workout duration, and calories burned.
3. **Correlation Analysis**: Identify relationships between workout type, frequency, and physiological markers.
4. **Age Group Analysis**: Group the dataset by age ranges to analyze trends across demographics.
5. **Gender Comparison**: Compare fitness habits and outcomes between
6. **Other Visualizations**: Create additional visualizations to explore the data further.
7. **Insights**: Provide insights based on the analysis.

## The Data

This dataset provides a detailed overview of gym members' exercise routines, physical attributes, and fitness metrics. It contains 973 samples of gym data, including key performance indicators such as heart rate, calories burned, and workout duration. Each entry also includes demographic data and experience levels, allowing for comprehensive analysis of fitness patterns, athlete progression, and health trends.

The dataset includes the following columns:

- `Age`: Age of the gym member.
- `Gender`: Gender of the gym member (Male or Female).
- `Weight (kg)`: Member’s weight in kilograms.
- `Height (m)`: Member’s height in meters.
- `Max_BPM`: Maximum heart rate (beats per minute) during workout sessions.
- `Avg_BPM`: Average heart rate during workout sessions.
- `Resting_BPM`: Heart rate at rest before workout.
- `Session_Duration (hours)`: Duration of each workout session in hours.
- `Calories_Burned`: Total calories burned during each session.
- `Workout_Type`: Type of workout performed (e.g., Cardio, Strength, Yoga, HIIT).
- `Fat_Percentage`: Body fat percentage of the member.
- `Water_Intake (liters)`: Daily water intake during workouts.
- `Workout_Frequency (days/week)`: Number of workout sessions per week.
- `Experience_Level`: Level of experience, from beginner (1) to expert (3).
- `BMI`: Body Mass Index, calculated from height and weight.

## Methodology

1. **Data Loading**: Load the dataset and examine its structure.
2. **Data Exploring**: Explore the dataset to understand the distribution of data.
3. **Descriptive Statistics**: Calculate key statistics to summarize the data.
4. **Exploratory Data Analysis (EDA)**: Analyze the data through visualizations and correlation analysis.
5. **Visualizations**: Create visualizations to present the findings effectively.
    - **Correlation Analysis**: Identify relationships between variables to uncover insights.
    - **Weight vs BMI Analysis**: Visualize the relationship between weight and BMI based on age group and gender group.
    - **Calories Burned Analysis**: Analyze the distribution of calories burned across different workout types and session durations.
    - **Heart Rate Analysis**: Examine the heart rate metrics and their relationship with workout type, workout frequency, and experience level.
    - **Water Intake Analysis**: Explore the water intake patterns and their impact on workout performance.

## Visualizations

### Correlation Analysis (Matrix)

![Correlation Matrix](https://i.imgur.com/tyyPy36.png)

**Key Observations**
- **Strong positive correlations**
   - `Calories_Burned` and `Session_Duration`: Longer sessions result in more calories burned.
   - `Water Intake` and `Workout Frequency`:  People who work out more frequently tend to drink more water.
   - `Experience Level and Workout Frequency`: More experienced individuals tend to work out more frequently.
   -  `Experience Level` and `Calories Burned`: More experienced individuals tend to burn more calories per session.
   - `Fat Percentage` and `Water Intake`: Higher water intake is associated with lower body fat percentage.
   - `BMI` and `Weight`: As expected, higher BMI is associated with higher weight.
   
- **Strong negative correlations**
   - `Water Intake` and `Fat Percentage`: Higher water intake is associated with lower body fat percentage.

**Implications**

- **Workout Intensity and Duration**: Focusing on longer, more intense workouts can lead to increased calorie burn. 
- **Hydration**: Prioritizing water intake, especially for those with higher workout frequency or body fat percentage, can be beneficial.
- **Experience and Results**: Encouraging consistent workout routines and progress tracking can lead to improved fitness levels and body composition. 
- **BMI Management**: A combination of increased physical activity, especially for experienced individuals, and a balanced diet can help manage BMI and body fat percentage. 

### Weight vs BMI based on Gender

![Weight vs BMI based on Gender](https://i.imgur.com/IVvaUx7.png)

- The scatter plot clearly shows a strong positive correlation between weight and BMI for both males and females. This means that as weight increases, BMI also tends to increase.
- While the overall trend is similar for both genders, there seems to be a slight difference in the distribution of points. Males tend to have higher BMI values for a given weight compared to females. This could be due to factors like muscle mass and body composition differences.
- The linear regression lines fit the data well, indicating that the relationship between weight and BMI is approximately linear for both genders.
- There are a few outliers in the data, especially for higher weight values. These could be due to individual variations in body composition or measurement errors.

### Weight vs BMI based on Age Group

![Weight vs BMI based on Age Group](https://i.imgur.com/EZDLUra.png)

- There's a clear positive correlation between weight and BMI across all age groups. This means as weight increases, BMI also tends to increase.
- While the overall trend is similar across age groups, there might be subtle differences in the distribution of points. For example, younger age groups might have a slightly lower BMI for a given weight compared to older age groups. This could be due to factors like muscle mass, body composition, and lifestyle differences.
- The linear regression line fits the data well, indicating that the relationship between weight and BMI is approximately linear across all age groups.
- There are a few outliers in the data, especially for higher weight values. These could be due to individual variations in body composition or measurement errors.

### Calories Burned Analysis

#### vs. Different Workout Types

![Calories Burned vs. Workout Type](https://i.imgur.com/wZYU0rM.png)

1. **Gender Differences**
   - Males generally burn more calories across all workout types compared to females. This could be attributed to factors like muscle mass and metabolic rate.
   - The difference in calorie burn between genders is most pronounced for HIIT and strength training workouts.

2. **Age Group Differences**-
   - Younger age groups (18-25, 26-35) tend to burn more calories, particularly during HIIT and strength training, compared to older age groups. This might be due to higher metabolic rates and physical activity levels in younger individuals.
   - Older age groups (56-65) tend to burn fewer calories across all workout types, possibly due to decreased muscle mass and metabolic rate.

3. **Experience Level Differences**
    - Individuals with higher experience levels tend to burn more calories compared to less experienced individuals. This could be due to factors like increased intensity, longer duration, and better workout efficiency.

#### vs. Session Duration

![Calories Burned vs. Session Duration](https://i.imgur.com/rqIYuhA.png)

1. **Gender Differences**
   - Both males and females exhibit a strong positive correlation between session duration and calories burned. This suggests that longer workout sessions generally lead to more calories burned.
   - The overall trend is similar for both genders, indicating that the relationship between session duration and calorie burn is consistent across genders.

2. **Age Group Differences**
   - All age groups show a positive correlation between session duration and calories burned.
   - There seems to be some variability in the spread of data points across age groups. Younger age groups might have a slightly wider range of calorie burn for a given session duration, potentially due to higher metabolic rates and physical activity levels.

3. **Experience Level Differences**
    - All experience levels show a positive correlation between session duration and calories burned.
    - More experienced individuals (level 3) tend to burn more calories for a given session duration compared to less experienced individuals. This could be attributed to factors like increased workout intensity, efficiency, and metabolic adaptation.

### Heart Rate Analysis

#### vs. Workout Type

![Heart Rate vs. Workout Type](https://i.imgur.com/LOSQJkq.png)

1. **Max BPM**
    - HIIT training tend to elicit higher maximum heart rates compared to Yoga and Cardio. This is expected as these workouts are more intense and demand greater cardiovascular effort.

2. **Avg BPM**
   - HIIT and Strength training again lead to higher average heart rates compared to Yoga and Cardio. However, the differences are less pronounced than for Max BPM.

3. **Resting BPM**
    - Resting heart rate is not significantly affected by workout type. It primarily reflects baseline cardiovascular fitness and overall health.

#### vs. Workout Frequency

![Heart Rate vs. Workout Frequency](https://i.imgur.com/aWNnFoD.png)

1. **Max BPM**
    - As workout frequency increases, Max BPM tends to decrease slightly. This could be due to the body's adaptation to regular exercise and a more efficient use of oxygen.

2. **Avg BPM**
   - Average heart rate also tends to decrease slightly with increasing workout frequency, indicating improved cardiovascular fitness and a more efficient heart rate response to exercise.

3. **Resting BPM**
    - Resting heart rate tends to decrease with increasing workout frequency. This is a positive indicator of improved cardiovascular health and fitness.

#### vs. Experience Level

![Heart Rate vs. Experience Level](https://i.imgur.com/75T2xKS.png)

1. **Max BPM**
    - There seems to be a slight decrease in Max BPM as experience level increases. This could be due to factors like improved cardiovascular fitness and a more efficient heart rate response to exercise.

2. **Avg BPM**
   - Average heart rate also tends to decrease slightly with increasing experience level, indicating improved cardiovascular fitness and a more efficient heart rate response to exercise.

3. **Resting BPM**
    - Resting heart rate tends to decrease with increasing experience level. This is a positive indicator of improved cardiovascular health and fitness.


### Water Intake Analysis

#### vs. Calories Burned

![Water Intake vs. Calories Burned](https://i.imgur.com/exXas2H.png)

- The scatter plot reveals a positive correlation between water intake and calories burned. This suggests that as individuals burn more calories, they tend to consume more water.
- The color coding based on experience level indicates that more experienced individuals (level 3) tend to drink more water, especially at higher calorie burn levels. This could be due to increased awareness of the importance of hydration, higher workout intensity, or longer workout durations.

#### vs. Fat Percentage

![Water Intake vs. Fat Percentage](https://i.imgur.com/e7fHYJ7.png)

- The data suggests that most athletes maintain a water intake between 2.0 to 3.5 liters regardless of their maximum heart rate, which ranges from 160 to 199 BPM. There's a notable consistency in the median water intake around 2.5-3.0 liters across different heart rate zones, though we see wider variations in some ranges, particularly around 170-175 BPM.
- There are a few outliers above 3.5 liters of water intake, specifically at heart rates of 177, 189, and 190 BPM, which could indicate individual hydration strategies during particularly intense training sessions. 
- The relatively stable water intake across different heart rate intensities suggests that athletes have developed personalized hydration protocols that they maintain regardless of exercise intensity.

## Results

The analysis of the gym members' exercise data has provided valuable insights into fitness patterns, calorie consumption, body composition, and workout outcomes. Key findings include:

1. **Correlation Analysis**: Identified strong positive correlations between variables such as calories burned and session duration, water intake and workout frequency, and experience level and workout intensity. Negative correlations were observed between water intake and fat percentage, highlighting the importance of hydration for body composition.
2. **Weight vs BMI Analysis**: Demonstrated a positive correlation between weight and BMI.
3. **Calories Burned Analysis**: Revealed differences in calorie burn based on workout type, session duration.
4. **Heart Rate Analysis**: Explored heart rate metrics across workout types, workout frequency, and experience levels.
5. **Water Intake Analysis**: Analyzed the relationship between water intake, calories burned, and fat percentage.

These insights can inform fitness planning, workout optimization, and health management strategies for gym members. By understanding the relationships between exercise habits, physiological markers, and fitness outcomes, individuals can make informed decisions to improve their overall health and well-being.

## Conclusion

The analysis of the gym members' exercise data has provided valuable insights into fitness patterns, calorie consumption, body composition, and workout outcomes. By exploring correlations between variables, visualizing trends across demographics, and comparing fitness habits and outcomes, we have gained a comprehensive understanding of the factors influencing exercise outcomes and fitness levels.
