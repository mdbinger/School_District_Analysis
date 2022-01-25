# School District Analysis
## Module 4 of Data Analytics Bootcamp
Maria is a Chief Data Scientist for the city school district. She has consulted us for help in analyzing the standardized test scores from all the schools in the city district and determining if any factors including school size, grade, school budget, etc., have any impact on student success on these standardized tests. We used the pandas tool within python on the platform Jupyter Notebook to write our code and perform our analyses. After we finished our original findings, we were informed all 9th grade test scores from Thomas High School needed to be voided and removed due to an issue involving academic integrity. We then ran the same analyses on the new data with the Thomas High 9th grade scores removed to see if there was any impact. 

# Results 
### Using bulleted lists and images of DataFrames as support, address the following questions.

#### 1) How is the district summary affected?
##### District Summary Including Thomas High 9th Graders
<img width="1012" alt="original_district_summary" src="https://user-images.githubusercontent.com/96350388/150896704-739ba540-44f8-42ca-99b3-b7e143f22c0c.png">

##### District Summary Excluding Thomas High 9th Graders
<img width="933" alt="new_district_summary" src="https://user-images.githubusercontent.com/96350388/150896765-bf9cfaa4-7dd1-44fa-8787-3c6ad55fb36d.png">

  - The average math score decreased by .1 overall when Thomas High School's 9th graders were removed
  - The average reading score was unaffected when Thomas High School's 9th graders were removed
  - The percent passing math, percent passing reading, and the overall percent passing were all unaffected when Thomas High School's 9th graders were removed
    - There may have been small changes similar to the average math score, but nothing large enough to result in the numbers being unequal when rounded to the nearest whole number as they are in our original district summary. 
  - Overall, it is safe to claim removing the Thomas High School 9th graders from our analysis did not significantly impact our district summary

#### 2) How is the school summary affected?
##### School Summary Including Thomas High 9th Graders
<img width="896" alt="original_school_summary" src="https://user-images.githubusercontent.com/96350388/150897481-10df4902-5f8f-499c-8683-4a10c070fc48.png">

##### School Summary Excluding Thomas High 9th Graders
<img width="893" alt="new_school_summary" src="https://user-images.githubusercontent.com/96350388/150897494-632645aa-2fcd-4d6a-863d-b750fe263715.png">

  - It might be obvious, but no schools were impacted by the removal of Thomas High School's 9th graders except for Thomas High School. Below is a summary of the impact that removing 9th graders had on Thomas High School:
    - Average math scores decreased from 83.418349 to 83.350937
    - Average reading scores increased from 83.848930 to 83.896082
    - The percent of students passing math decreased from 93.272171 to 93.185690
    - The percent of students passing reading decreased from 97.308869 to 97.018739
    - The percent of overall students passing decreased from 90.948012 to 90.630324
    - These changes are all very small and not very noteworthy. However, it is interesting that despite 9th graders being removed for academic integrity, the average reading scores increased when the 9th grade scores were removed. This was not expected, as typically academic integrity violations are designed to increase scores, so you would expect the average reading scores to be lower when those scores were removed, just like all the other categories were. 

#### 3) How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
  - Looking at the school summaries above from 2), we can see that both before and after the scores were removed, Thomas High School was one of the best performing schools in the district. Both with and without the 9th grade scores, Thomas High School is the 2nd highest performing school in the district based upon percentage of students overall passing, so again there isn't really impact resulting from dropping the 9th grade scores. 

#### 4) How does replacing the ninth-grade scores affect math and reading scores by grade
##### Original Math Scores by Grade
<img width="265" alt="original_math_scores_by_grade" src="https://user-images.githubusercontent.com/96350388/151062841-d5ab2075-4252-4f29-aa2b-07e1b1dddf3a.png">

##### Original Reading Scores by Grade
<img width="264" alt="original_reading_scores_by_grade" src="https://user-images.githubusercontent.com/96350388/151062858-cce8a7bf-fc31-4a14-ab93-4cd04d166297.png">

##### New Math Scores by Grade Without Thomas High 9th Graders
<img width="670" alt="new_math_scores_by_grade" src="https://user-images.githubusercontent.com/96350388/151062968-b65437a2-78ec-4bfc-a694-ca255f12c0e6.png">

##### New Reading Scores by Grade Without Thomas High 9th Graders
<img width="735" alt="new_reading_scores_by_grade" src="https://user-images.githubusercontent.com/96350388/151063056-bfc646a6-797b-4adc-87b6-e9afb2daf63a.png">

  - There is no impact on any scores for reading or math, other than the scores that were removed. This is because the 9th grade reading and math scores from Thomas High School are independent data points relative to the entire data frame, meaning that changing them will have no impact on the other data in the data frame.

#### 5) How does replacing the ninth-grade scores affect scores by school spending
##### Original Scores by School Spending
<img width="728" alt="original_scores_by_spending" src="https://user-images.githubusercontent.com/96350388/151063902-1a49ff90-8b83-4b6b-ac0f-53fe220b2611.png">

##### Scores by School Spending After Thomas High School 9th Grade Scores Removed
<img width="731" alt="new_scores_by_spending" src="https://user-images.githubusercontent.com/96350388/151063923-ef6dc10b-6bf6-436c-934f-3cb48e06faf5.png">

  - Similar to what we saw in 1), the rounding was different in our original analysis compared to the new analysis after removing 9th grade scores from Thomas High School. 
  - Thomas High School fell into the $630 - $644 spending category, so if there were to be differences caused by dropping the 9th grade scores we would expect the $630 - $644 numbers to differ and not any others. 
  - That said, if the scores are all rounded to the nearest tenth decimal point and the percentages are all rounded to the nearest whole number (as they are in the new analysis), all the numbers would be the same, so we can safely say dropping the 9th grade scores had no impact on our summary by school spending.

#### 6) How does replacing the ninth-grade scores affect scores by school size

#### 7) How does replacing the ninth-grade scores affect scores by school type


# Summary 
### Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.
