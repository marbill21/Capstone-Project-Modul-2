# Capstone-Project-Modul-2
Name : Mario Billy Gunawan <br>
Student ID : JCDSOL-009-022 <br>
Topic : [Crime in Boston](https://www.kaggle.com/datasets/AnalyzeBoston/crimes-in-boston) 
<hr>

## Project Guideline
In Module 2: Data Analysis, students have learned about SQL, data manipulation, data visualization, and statistics. The Capstone Project for Module 2 aims to implement the knowledge acquired by students into a project.

The goal of the Capstone Project is to train students in conducting a series of analyses. In this project, students will assume the role of a data analyst in a company. They will formulate a set of questions based on the business needs and potential challenges faced by the company, using the available data.

Students will answer these questions through data analysis, create narratives and visualizations, and present insights from their analysis. These insights can then serve as a basis for business decision-making by stakeholders.

At the end of the project, students are required to submit 3 files: a documented analysis in a Jupyter Notebook, a story created in Tableau Public, and 1 video explaining the problem and the analysis performed.

<hr>

## Project Presentation
Slide 1
![Crime_in_Boston](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_1.png)
- The topic that I received to work on for Capstone Project Module 2 is "Crime in Boston." <br>

Slide 2
![Table_of_Contents](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_2.png)
- The table of contents for this presentation begins with identifying the data profile, formulating the problem, outlining insights and recommendations, and finally drawing conclusions from this data analysis.

Slide 3
![Involved_Parties](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_3.png)
- In this data analysis, there are two parties involved. The first party is myself, Mario Billy Gunawan, as the Data Analyst Consultant. The second party is the Boston Police Department, who acts as the user or client.

Slide 4
![Data_Profile](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_4.png)
- The datasets used in this data analysis consist of 2 files, namely crime.csv and offense_codes.csv.
- The data collection period spans from June 14, 2015 to September 3, 2018.
- The data was collected in the city of Boston, Massachusetts, United States.
- The source of the datasets is from the website Kaggle.com.

Slide 5
![Columns](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_5.png)
In this dataset, the columns can be described as follows:

- The `INCIDENT_NUMBER` column represents a unique number for each incident that occurred in the city of Boston. Meanwhile, the `OFFENSE_CODE` column represents the code for the type of offense. These two columns are then combined to create a new index representing each incident and its associated offense in Boston.
- Offense Detail: It consists of the `OFFENSE_CODE` column (code for the type of offense group), `OFFENSE_CODE_GROUP` column (name of the offense code group), and `OFFENSE_DESCRIPTION` column (description of the offense that occurred).
- Incident Location: It consists of the `DISTRICT` column (code for the district where the incident occurred), `DISTRICT_NAME` column (name of the district where the incident occurred), and `Location` column (coordinates - latitude and longitude - of the incident location).
- Incident Details: It consists of the `DATE` column (date of the incident), `TIME` column (time of the incident), `SHOOTING` column (N - No shooting incident, Y - Shooting incident occurred), and `UCR_PART` column (ranking of the most serious offense type per incident).
- Unutilized Column: Columns that are eliminated or not used. It includes the `REPORTING_AREA` column (code for the reporting area of an incident) and the `STREET` column (name of the street where the incident occurred). These two columns cannot be linked to data in other columns, making them irrelevant for analysis.

Slide 6
![Background](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_6.png)
- The background for conducting this data analysis is based on an article stating that there was a 54% surge in homicide incidents in 2020, with a total of 57 cases compared to the previous year, which had only 37 incidents. This number of incidents in 2020 became the lowest in the last 20 years.

Slide 7
![Problem_Statements](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_7.png)
- The following is a statement of the problem created to assist in analyzing this data:
  
Slide 8
![Insights&Recommmendation](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_8.png)
- In this stage, we will examine the insights that can be obtained from the data analysis. Based on these insights, recommendations will be provided to help address the existing issues or improve the performance of the insights if they are already good.

Slide 9
![I&R_1a](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_9.png)
- Here are the top 5 incident types with the highest count and percentage:

Slide 10
![I&R_1b](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_10.png)
- The most frequently reported incident type is providing medical assistance to the sick or injured, with a total of 18,783 incidents, accounting for 5.89% of the total incidents.
- The first recommendation is to provide basic first aid training to every patrol officer. This is also aimed at anticipating delays in medical assistance at the scene of accidents.
- Additionally, it is advisable to equip each police patrol car with a first aid kit (P3K) so that it can be used in case of accidents.

Slide 11
![I&R_2a](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_11.png)
- The following is a map of Boston City divided into 12 districts. The darker the color of a district, the higher the number of incidents that occurred in that district.
- There are also 10 blue pinpoint markers indicating the 10 locations with the highest total incidents in Boston.

Slide 12
![I&R_2b](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_12.png)
- It can be observed that the highest number of incidents occurred in Roxbury District (B2) with a deep red color indicating 49,939 incidents, accounting for 15.74% of the total incidents.
- On the other hand, the lowest number of incidents occurred in Charlestown District (A15) with a light cream color indicating 6,505 incidents, accounting for 2.04% of the total incidents.
- There are also 4 locations with the highest total incidents clustered in 3 different districts, namely Roxbury (B2), South Boston (C6), and South End (D4).
- The recommendation is to increase personnel and patrol schedules to monitor the 5 districts with a significant number of incidents ranging from 35,000 to 49,000, namely Roxbury (B2), Dorchester (C11), South End (D4), Downtown (A1), and Mattapan (B3).
- The Boston Police Department (BPD) is also advised to establish a special task force to investigate whether there are any connections or correlations among the 4 locations with the highest total incidents clustered in 3 different districts. This will help determine if there is an organized criminal group in the area or if it is merely a coincidence that they are close to each other.

Slide 13
![I&R_3a](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_13.png)
- The following is the trend pattern of the total homicide and shooting incidents that occurred in the city of Boston from 2015 to 2018.

Slide 14
![I&R_3b](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_14.png)
- The number of shooting and homicide incidents showed a fluctuating trend from 2015 to 2018. During the period from 2015 to 2017, the number of incidents increased, while there was a significant decrease in incidents from 2017 to 2018.
- This indicates that preventive and repressive measures against firearm use can be considered successful in reducing shooting-related crimes by up to 185 incidents.
- In 2018, there were 33 homicide cases, but in 2020, there was a 54% surge compared to the previous year, with 37 incidents. Indirectly, this suggests that incidents involving the use of firearms also increased.
- A recommendation to the Boston Police Department is to review the preventive and repressive strategies that were previously successful from 2017 to 2018. There is a possibility that illegal firearms have become more accessible again, and there might be a relaxation in monitoring gang members. Inter-gang conflicts could be one of the factors contributing to the increase in homicide incidents.

Slide 15
![I&R_4a](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_15.png)
- The following is the proportion of each day of the week for every incident that occurred in the city of Boston.

Slide 16
![I&R_4b](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_16.png)
- Based on the pie chart, it can be observed that violation incidents in Boston occur most frequently on Fridays, accounting for 15.20% of the total. Wednesdays and Thursdays follow closely, with percentages of 14.65% and 14.62% respectively.
- Saturdays and Sundays are the days with the least violation incidents, accounting for 14.05% and 12.64% respectively.
- This indicates that violation incidents in Boston tend to occur more on weekdays compared to weekends.
- The Boston Police Department (BPD) is advised to reevaluate the schedule of police personnel patrols. Patrol activities on Wednesdays, Thursdays, and Fridays should be prioritized over Saturdays and Sundays. By adding more patrols on these days, it is hoped that the number of incidents per day can be reduced, creating a safer environment for the residents of Boston.

Slide 17
![I&R_5a](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_17.png)
- The following is the result of the hypothesis test and graph analysis to determine if there is a tendency for more incidents to occur at night. The hypothesis test result shows rejecting H0, which means that violation incidents are not significantly more likely to occur 50% more at night.

Slide 18
![I&R_5b](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_18.png)
- Based on the hypothesis test and the previous pie chart analysis, it can be observed that the proportion of incidents occurring at night is not significantly higher compared to the daytime. This might be influenced by the reduced activities of residents during the night.
- However, the decreased activities during the night also create opportunities for criminals to carry out their actions. For example, incidents like home burglaries often occur at night when many residents are asleep, providing the perpetrators with a greater chance to commit the crime unnoticed.
- Although the proportion of incidents is higher during the daytime, the proportion of incidents occurring at night is still significant, accounting for 37.44%. Therefore, the Boston Police Department is advised to increase personnel and patrol routes during the night, especially in areas with a higher risk of criminal incidents, as mentioned in the analysis point number 2. This increased presence can help deter criminal activities and ensure the safety of the residents during nighttime hours.

Slide 19
![I&R_6a](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_19.png)
- The following is the ranking of UCR categories with the highest number of incidents, along with the top 3 incident types in each UCR_Part category based on their occurrences.
Slide 20
![I&R_6b](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_20.png)

Slide 21
![I&R_6c](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_21.png)

Slide 22
![I&R_6d](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_22.png)
- Based on the overall cross-tabulation, it can be seen that the largest percentage of incidents belongs to UCR Part 3, with a value of 49.69% and a total of 158,537 incidents.
- The most frequent Uniform Crime Reporting (UCR) Part 1 incident in Boston is theft inside buildings with stolen goods valued above $200, with a percentage above 12%.
- The most frequent Uniform Crime Reporting (UCR) Part 2 incident in Boston is vandalism or graffiti on other people's property without the owner's permission, with a percentage above 15%.
- The most frequent Uniform Crime Reporting (UCR) Part 3 incident is providing medical assistance to the sick or injured, accounting for 11.85%.
- The "Other" category in the Uniform Crime Reporting (UCR) reports comprises over 85% of all incidents in this UCR type and involves the return of stolen motor vehicles by the police outside Boston.
- The "N/A" category in the Uniform Crime Reporting (UCR) reports comprises over 89% of all incidents in this UCR type and involves unlawfully entering someone else's home without the owner's permission.
- According to the [Wikipedia page on Uniform Crime Reports](https://en.wikipedia.org/wiki/Uniform_Crime_Reports), criminal offenses are only divided into two main groups: Part 1 Offenses and Part 2 Offenses. Therefore, the Boston Police Department (BPD) should reconsider its classification of incidents in the city. As per the reference, the FBI categorizes the Uniform Crime Report (UCR) into only 2 parts, Part 1 and Part 2. However, the Boston Police Department (BPD) divides the UCR category into 3 parts and includes 2 other categories, namely "Other" and "N/A".

Slide 23
![Conclusion](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_23.png)
- Basic first aid training should be provided to police patrol personnel, and first aid kits (P3K) should be made available in every patrol vehicle.
- There is a need to increase the number of police patrol personnel, revise patrol schedules and routes, especially on Wednesdays, Thursdays, and Fridays, and during nighttime in the districts with the highest risk of criminal incidents.
- The preventive and repressive strategies regarding the use of firearms should be reviewed, as there was a 54% surge in homicide incidents in 2020 compared to the previous year, with 57 cases recorded in contrast to 37 cases. The trend in shooting and homicide incidents from 2015 to 2018 also showed a similar pattern.
- The classification of UCR categories by the Boston Police Department needs to be reconsidered because based on the official categories issued by the FBI, UCR is only categorized into two main groups: UCR Part 1 and UCR Part 2.

Slide 24
![Thank_You](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_24.png)
- That's the end of my data analysis presentation on Crime In Boston. Thank you for your time and attention.




















