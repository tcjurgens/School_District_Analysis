# School District Analysis 
## Overview
The purpose of this analysis was to review school performance based on a variety of factors. These factors being: 
- school size (small,medium,large)
- school type (district, charter)
- school spending

We judge performace based on the students scores and passing rates for math and reading. 

In this challenge, we were concerned about academic dishonesty from the ninth grade at Thomas High School. Because of this concern, we refactored the code we worked on in the module to not include any math/reading scores from the 9th grade at Thomas in our analysis.

## Results
Shown below are certain comparitive results of the analysis in PyCitySchools_Challenge.ipynb compared to PyCitySchools.ipynb (the challenge file has scores from the 9th grade at Thomas High School excluded). 
the line of code used to calculate the total number of 9th graders at Thomas High School is: len(student_data_df.loc[(student_data_df["school_name"] == 'Thomas High School') & (student_data_df["grade"] == '9th')])  
This code lets us know that there are 461 9th graders at Thomas High which should not be accounted for in the Challenge Analysis

<img width="778" alt="Screen Shot 2021-07-23 at 7 42 52 PM" src="https://user-images.githubusercontent.com/86446641/126850587-a5200520-a011-45a1-8858-23a26a933c28.png">


You can see that when the 461 9th graders are accounted for we have a slightly lower passing percentage for both subjects in the district.

Further; if we focus specifically on Thomas High School, the passing percentages are much more drastic. 
<img width="367" alt="Screen Shot 2021-07-19 at 10 20 08 AM" src="https://user-images.githubusercontent.com/86446641/126175172-4c1ef0c4-fe20-4da2-96a8-6726adbf1eee.png">
<img width="357" alt="Screen Shot 2021-07-19 at 10 20 57 AM" src="https://user-images.githubusercontent.com/86446641/126175290-7c708635-3cf1-474e-a9d0-97d828e43f1f.png">

These two above images show the difference in passing percentages specifically at Thomas High with 9th grade scores first excluded and then included. You can see the differences reflected in % and in the total students count. The results are significant. 


