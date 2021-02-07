# School District Analysis
## Overview
Previously, our client, Maria, a data engineer for an undisclosed school district, tasked us with aggregating district data and providing insights to the superintendent and school board about school performance trends and patterns in order to make decisions on school budgets and priorities. In particular, we looked at student funding and student test scores, using math and reading scores, as well as various information on the schools they attend, such as school size and type.

### Scope of current analysis: an addendum
Due to awareness of dishonesty in the reporting of the math and reading grades for Thomas High School (THS) ninth graders, and the school board wanting to uphold state-testing standards, Maria asked us to remove THS grades, while keeping the rest of the data intact, and to repeat the school district analysis and report how these changes affected the overall analysis.

## Results
### How replacing the ninth graders’ math and reading scores affect the school district numbers 
*	**District Summary:** All but one aptitude-based result dropped by a small margin, while the average reading score remained the same. The passing reading percentage experienced the greatest drop at three-tenths of a point (85.7% from 86%). 
##### Original
![District Summary: before](https://github.com/andeevosters/School_District_Analysis/blob/main/Resources/Screenshots/district_summary_df_after.png)
 
##### Altered
![District Summary: after](https://github.com/andeevosters/School_District_Analysis/blob/main/Resources/Screenshots/district_summary_df_after.png)
 
**School summary** (ranked by percentage of students passing both math and reading):*
  *	The five schools with the highest percentage of students passing both math and reading are as follows, in order (highest to lowest): Cabrera High School (91.33%), Thomas High School (90.63%), Griffin High School (90.60%), Wilson High School (90.58%), and Pena High School (90.54%).
  *	On the contrary, the five schools with the lowest percentage of students passing both math and reading are as follows, in order (lowest to highest): Rodriguez High School (52.99%), Figueroa High School (53.20%), Huang High School (53.51%), Hernandez High School (53.53%), and Johnson High School (53.54%).
  *	There was a 37.79-point spread between the highest-performing school (Cabrera High School, 91.33%) and the lowest-performing school (Johnson High School, 53.54%).

**Thomas High School’s performance relative to the other schools:**
  *	Thomas High School is the second-highest-performing high school in the district (90.63%). That rank did not falter after eliminating the ninth-graders’ grades from the results, however it did drop from 90.94%, or nearly 1/3 percent.

**Math and reading scores by grade:**
  *	Before eliminating THS 9th graders’ math grades: 9th graders held the highest math passing percentage in their school (83.6%), followed by 12th graders (83.5%).
  *	Before eliminating THS 9th graders’ reading: THS 9th graders held the third highest reading passing percentage in their school (83.7%), behind 10 graders (84.3%) and 12th graders (83.8%).

**Scores by school spending:** Eliminating THS’ 9th-grade scores did not affect the overall scores, and therefore did not affect the school spending results. Below are the results.
![Scores by School Spending](https://github.com/andeevosters/School_District_Analysis/blob/main/Resources/Screenshots/spending_summary_df_after.png)

**Scores by school size:** Scores by school size were also not affected by eliminating THS’ 9th-grade scores. Below are the results.
![Scores by School Size](https://github.com/andeevosters/School_District_Analysis/blob/main/Resources/Screenshots/size_summary_df_after.png)

**Scores by school type:** Scores by school type were also not affected by eliminating THS’ 9th-grade scores. Below are the results.
![Scores by School Type](https://github.com/andeevosters/School_District_Analysis/blob/main/Resources/Screenshots/type_summary_df_after.png) 


## Summary
1.	Overall, eliminating Thomas High School’s 9th graders’ grades did not significantly impact the overall results. Rather, minimal, if any numbers varied.
2.	District-wide, the passing reading percentage experienced the greatest drop at three-tenths of a point (85.7% from 86%). 
3.	Before eliminating THS 9th graders’ math grades: 9th graders held the highest math passing percentage in their school (83.6%), followed by 12th graders (83.5%).
4.	Before eliminating THS 9th graders’ reading: THS 9th graders held the third highest reading passing percentage in their school (83.7%), behind 10 graders (84.3%) and 12th graders (83.8%).

## Resources
Software: Jupyter Notebook 6.1.4, Python 3.8.5, Anaconda 1.7.2,
Data Sources:
•	Data Analysis: PyCitySchools_Challenge, PyCitySchools
•	Raw data: students_complete.csv, schools_complete.csv
