# School_District_Analysis
School standardized testing using Anaconda, jupyter lab and jupyter notebook via python. 

### Deliverable 3: A Written Report for the School District Analysis (25 points)
# Deliverable 3 Instructions
For this part of the Challenge, write a report that summarizes your updated analysis and compares it with the results from the module.


## Overview of the school district analysis: Explain the purpose of this analysis.
The purpose of this analysis is to analyze the standardized testing resultes of 15 different high schools, comparing test scores from reading and math tests for 9th to 12th graders. In the challenge, Maria notified us that test results for Thomas High School (THS) 9th graders have been altered. We replaced the THS's 9th grade test results with NaNs while maintaining the rest of the datasety, and then repeated the school district analysis that we completed in the module. 


## Results: Using bulleted lists and images of DataFrames as support, address the following questions.

# How is the district summary affected?
The module district summary dataframe appears like this: 
<img width="794" alt="Screen Shot 2022-01-18 at 7 25 05 PM" src="https://user-images.githubusercontent.com/96043107/150051935-842284e4-8107-48c3-9ddf-6fa7931fcaa1.png">

The challenge district summary dataframe looks like this:
<img width="631" alt="Screen Shot 2022-01-18 at 7 23 12 PM" src="https://user-images.githubusercontent.com/96043107/150051716-87638ef7-0da6-4eaf-88bf-494177cb31e7.png">
Not much changed, other than the overall passing percentage and the reading passing percentage decreased when we excluded THS's 9th grade results.

# How is the school summary affected?
All of the schools in the school summary are unaffected, except for THS, where the average reading and math scores remained very similar between the challenge and module datasets. Also, the percent passing math, reading, and overall passing figures decreased significantly between the module and challenge datasets by about 25-30% in each category. 

# How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
THS' performance compared to the other schools after replacing the 9th graders reading and math scores are generally lower than the average math, reading, and overal passing percentages of other high schools. 

<img width="717" alt="Screen Shot 2022-01-18 at 8 11 10 PM" src="https://user-images.githubusercontent.com/96043107/150056902-efcdbee8-bc13-473a-9130-8af1e5ffc57b.png">
As you can see in the image above, THS's scores of 66.9%, 69.7%, and 65.1% in math, reading, and overall passing percentages, respectively, are generally lowerthan other high school's performances. 

# How does replacing the ninth-grade scores affect the following:
# Math and reading scores by grade
Math and reading scores by grade are only impacted by the omission of THS' 9th grade scores.. this action does not impact any of the other math and reading scores by grade. Images of the dataframes for reading and math scores are shown below, with "nan" replacing THS' 9th grade scores. 
<img width="277" alt="Screen Shot 2022-01-18 at 8 25 05 PM" src="https://user-images.githubusercontent.com/96043107/150058286-5062bcb7-e084-41d9-9953-853bbd07a648.png">

<img width="276" alt="Screen Shot 2022-01-18 at 8 25 20 PM" src="https://user-images.githubusercontent.com/96043107/150058309-119567fd-2657-4e2b-baae-5e881b55187d.png">



# Scores by school spending
Scores by school spending only affects the spending bracket that THS is in, which is the $630-$644 bracket. After examining the dataframes for the spending ranges between the module and the challenge, I find that the categories average math score, average reading score, percent passing math, percent passing reading, and percent overall passing did not change by over a percent difference. 

# Scores by school size
Again, since we only excluded the 9th graders reading and math scores from one out of the fifteen highschools we're examining, the data between the module dataframe and the challenge dataframe is largely unaffected, only changing the scoring categories minisculely. Only scoring figures from schools in the "medium (1000-2000)" size range will be affected since THS is a medium sized school, and the results, when rounded to the nearest tenth for average score, and nearest whole number for passing percentages, are not impacted. 

# Scores by school type
Since there are only two different school type categories, Charter and District, we know that the exclusion of THS' 9th grade scores are hardly going to impact the differences in scores betwewen the two school types, with there being 7 "District" schools, and 8 "Charter" schools. THS is a Charter school, so excluding the 9th graders reading and math scores from the 8 other schools that are Charter schools has very little effect on the differences in average math score, average reading score, and passing score percentages between the challenge school type dataframe and the module school type dataframe. Screenshots of the two data frames from the challenge school dype dataframe and the module school type dataframe are included below. 

Challenge (THS 9th grade scores excluded): 
<img width="563" alt="Screen Shot 2022-01-19 at 8 10 46 AM" src="https://user-images.githubusercontent.com/96043107/150158611-23b081ed-9145-40ad-899b-3f83003906d3.png">

Module (THS 9th grade scores included):
<img width="568" alt="Screen Shot 2022-01-19 at 8 11 25 AM" src="https://user-images.githubusercontent.com/96043107/150158742-4542dde5-49be-48e3-bc45-2f9dcb883e92.png">


## Summary: Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.

Overall, replacing THS' 9th grade math and reading test results with NaNs only significantly impacted when comparing THS' average percentage grade in the overall, in math, and reading categories. The other ways we organized the data, such as comparing the school types, school sizes, and school spending categories were largely unchanged between the challenge and module datasets. This was because dropping the 9th grade THS students scores was not enough data to shift the average math and reading scores, as well as percent passing calculations. 
