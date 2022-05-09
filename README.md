# School_District_Analysis
School_District_Analysis
## Project Overview
The purpose of this project is to analyze math and reading scores of Thomas High School 9th grade students and determine whether or not there was any academic dishonesty. Data set has been collected from several schools in the district which will be used in comparison to prove or reject if Thomas High School test results have been altered or manipulated in any way. There are two main datasets used during this project; school data (name of the school, type of school, school size, and budget) and student data (school, name, grade, and test scores). I managed to merge the datasets to view summaries, trends, performance, and test scores. By doing so, I would be able to identify anomalies and analyse the data before and after making this change.

* The district summary
* The school summary
* The top 5 and bottom 5 performing schools, based on the overall passing rate.
* The average math score for each grade level from each school
* The average reading score for each grade level from each school
* The scores by school spending per student, by school size, and by school type

## Resources
- Data Source: schools_complete.csv, students_complete.csv
- Sofware: Jupyter Notebook 6.4.5
- Library: Pandas, Numpy
- Language: Python 3.9.7

## Analysis Results

### Impact on District Analysis
*District Summary Before*

![District Summary Before]

*District Summary After*

![District Summary After]

- The data did not have affected in terms of Total Schools, Total Students and Total Budget.
- `Average Math scores` decreased by 0.1% from 79 to 78.9 and `Average Reading scores` did not change.
- `Percent Passing Math` decreased by 0.2% from 75 to 74.8, `Percent Passing Reading` decreased by 0.1% from 85.8 to 85.7 and `Percent Overall Passing` decreased by 0.3% from 65.2 to 64.9

### Impact on the School Summary 
*School Summary Before*

![Per_School_Summary_Before]

*School Summary After*

![Per_School_Summary_After]

- `Average Math` at Thomas High School decreased from 83.42 to 83.35 and `Average Reading` at Thomas High School slightly increased from 83.85 to 83.90.
- `Percent Passing Math` at Thomas High School greatly decreased from 93.27% to 66.91%, `Percent Passing Reading` at Thomas High School decreased from 97.31% to 69.66% and `Percent Overall Passing` at Thomas High School decreased from 90.95% to 65.08%.

### Replacing the ninth graders’ math and reading scores affected Thomas High School’s performance relative to the other schools
Replacing the ninth graders' math and reading scores with Nan values affects drastically Thomas High School's performance relative to the other schools by showing that Passing students for Math and Reading decread almost 27 -28% and Overall Passing students dropped to almost 25-26%.
![Excluding_False_Data]

While the average math, reading and overall scores at Thomas High School were impacted with the update, the changes only had a small impact.
![Top_School_Original]

![Top_School_Updated]

### Replacing the ninth-grade scores affect the following:
* Math and reading scores by grade:
The data simply becomes `nan` when replacing the ninth-graders scores affects the math and reading scores by grade simply by excluding the data for that column for that specific grade and that specific school.

*Math Scores Before & After*

![Math_scores_Before]


![Math_scores_After]

*Reading Scores Before & After*

![Reading_scores_Before]


![Reading_scores_After]


*Scores by school spending Before & After:
Thomas High School fell in the category of spending range per student of $631- $645,

![School_Spending_Before]


![School_Spending_After]


*Scores by school size Before & After:
Thomas High School fell in the Medium Category(1000-2000),

![School_Size_Before]

![School_Size_After]


*Scores by school type Before & After:
Thomas High School fell in the Charter category,

![School_type_Before]

![School_type_After]


## Summary: 
The changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.
*There was not a major difference in total District performance when Thomas High School 9th grade students scores were removed (Nans). Math, Reading, and overall results had either no impact or at most 1% difference. 
*There were significant changes to Thomas High School performance when 9th grade data was removed for Math, Reading, and total scores. On average results decreased by 25%. 
*Thomas High School ranking was impacted as well, it went from 2nd place to 8th place in the District. 
*Data clearly shows Charter schools performed much better compared to District schools in every measurable category.  
*It is also clear Large schools (2000-5000) had the worst scores. Small and Medium size schools had higher scores.  

