# School_District_Analysis

## Overview of the Analysis
The purpose of this analysis was to help the school board analyze the high schools in the district based on a variety of metrics. When the school board notified us of the academic dishonesty from the 9th grade students at Thomas High School, I had to refactor the code to adjust out the math and reading scores for those students. 

## Results
- The district summary was affected by removing the 9th grade students scores from Thomas High School. I used `.loc` and .`count()` in order to find the number of 9th grade students from Thomas High school. Next, I had to adjust the total number of students in the district to remove these students `thomas_hs_count_new = thomas_hs_count_total - student_9th_count`. The passing percentages for math and reading both decreased slightly after removing the 9th grade students. This makes sense because if the students cheated on their tests, their scores would be higher and more likely to score a passing grade, so removing them would lower the percentages for the district. 
- For the school summary, the only school that was affected by removing the 9th grade students was Thomas High School. 
- Replacing the ninth graders' math and reading scores lowers Thomas High School's performance relative to the other schools. 
- When you look at the math and reading scores by grade, the only thing that changes is for 9th grade students at Thomas High School. Where there was once an average, it now outputs `NaN`.
- The scores by school spending does not change.
- The scores by school size does not change.
- The scores by school type does not change. 

## Summary
Changing Thomas High School's 9th grade students scores to `NaN` lowered the passing percentages for the district summary, school summary, and the performance of Thomas High School relative to the other high schools. It did not effect the 
analsys when categorizing the data into bins by grade, school spending, school size, and school type. 