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

<img width="1022" alt="Screen Shot 2021-07-19 at 10 04 04 AM" src="https://user-images.githubusercontent.com/86446641/126172679-c47337ba-eae4-45bd-835b-02ebb006b775.png">
above shows the percent of students who passed math and reading w the 9th graders at Thomas High excluded, and below shows the results when the 9th graders are accounted for in the data.
<img width="1018" alt="Screen Shot 2021-07-19 at 10 05 24 AM" src="https://user-images.githubusercontent.com/86446641/126172895-7611ebe1-901d-45f7-9ce8-72ee2a46fcb3.png">

You can see that when the 461 9th graders are accounted for we have a slightly higher passing percentage for both subjects in the district.


