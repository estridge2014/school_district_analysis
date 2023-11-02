# CUNY Portfolio Example #2: School District Analysis 

### Context of the project

The school board has notified Maria and her supervisor that the [students_complete.csv](https://github.com/estridge2014/school_district_analysis/blob/main/resources/students_complete.csv)
 file shows evidence of academic dishonesty; specifically, reading and math grades for Thomas High School ninth graders appear to have been altered. Although the school board does not know the full extent of the academic dishonesty, they want to uphold state-testing standards and have turned to Maria for help. She has asked you to replace the math and reading scores for Thomas High School with NaNs while keeping the rest of the data intact. Once you’ve replaced the math and reading scores, Maria would like you to repeat the school district analysis that you did in this module and write up a report to describe how these changes affected the overall analysis.

### Shortened analysis description 
Find the completed School District Analysis code [here](https://github.com/estridge2014/school_district_analysis/blob/main/PyCitySchools_Challenge.ipynb) for reference.

1. In the district summary, the Percent Overall Passing Reduced by 0.3%

2. In the school summary, the Percent Overall Passing for Thomas High School reduced by 0.3%

3. After removing the testing scores of the 461 ninth graders at Thomas High School, passing percentages of the school did end up being lowered, but not by much (each less than 1%).

Math score average

*Original: 93.27

*Updated: 93.18

Reading score average 

*Original: 97.3

*Update: 97.01

Overall score average

*Original: 90.948

*Updated: 90.63

4. After replacing the invalid scores from the Thomas High School 9th grade class with NaN, the overall summary changes slightly (likely because 9th graders at Thompson High School is such a small portion of the overall scores). Originally, the overall passing score was 65.172. After recalculating and rounding it to the nearest tenth, it is 64.9% overall passing rate. The original passing rate for reading was 85.8% and was lowered to 85.7% when the averages were recalculated. The original passing rate for math was 74.98% and was lowered to 74.8% after recalculating.

![Original_district_summary](https://github.com/estridge2014/school_district_analysis/assets/84936545/e98eec6e-19d8-4826-89db-300fe5f5d4c7)

Updated district summary

<img width="644" alt="Screen Shot 2021-07-11 at 3 24 16 PM" src="https://user-images.githubusercontent.com/84936545/125207770-1c06ac00-e25c-11eb-88fc-b579527e9912.png">
   
It is difficult to come to a conclusion about academic dishonesty for Thomas High School 9th grade math and reading scores based on this analysis. When omitting the 9th grade scores, Thomas High School % passing math, % passing reading and % overall passing were reduced by <1%. This is not a large enough margin to determine academic dishonesty. Further tests will need to be implemented for a stronger conclusion.

### End of portfolio example

---------------------------

## Overview: 

After previously calculating the results of the state testing scores for both the overall district and schools individually, we have become aware that the scores for the 9th grade class at Thomas High School appear to be altered. In order to address this issue, and ensure that our final analysis is as accurate as possible, we have chosen to remove those scores from the final analysis calculations and replace them with N/A.     

## Process: 

Deliverable 1: We found and replaced the Thomas High School ninth-grade reading and math scores with "NaN" values before running the school district analysis

Deliverable 2: We repeated the school district analysis using our new DataFrame and updated the following summaries:

1. The district summary
2. The school summary
3. The top 5 performing schools, based on the overall passing rate
4. The bottom and 5 performing schools, based on the overall passing rate
5. The average math score for each grade level from each school
6. The average reading score for each grade level from each school
7. The scores by school spending per student, by school size, and by school type

## Resources 

Data Sources: [schools_complete.csv](https://github.com/estridge2014/school_district_analysis/blob/main/resources/schools_complete.csv) , [students_complete.csv](https://github.com/estridge2014/school_district_analysis/blob/main/resources/students_complete.csv)

Software: Python 3.7.6, Conda 4.10.1

Environment: Jupyter Notebook

## How is the district summary affected?

After replacing the invalid scores from the Thomas High School 9th grade class with NaN, the overall summary changes slightly (likely because 9th graders at Thompson High School is such a small portion of the overall scores). Originally, the overall passing score was 65.172. After recalculating and rounding it to the nearest tenth, it is 64.9% overall passing rate. The original passing rate for reading was 85.8% and was lowered to 85.7% when the averages were recalculated. The original passing rate for math was 74.98% and was lowered to 74.8% after recalculating. 

### Original district summary 

![Original_district_summary](https://github.com/estridge2014/school_district_analysis/assets/84936545/e98eec6e-19d8-4826-89db-300fe5f5d4c7)

### Updated district summary

<img width="644" alt="Screen Shot 2021-07-11 at 3 24 16 PM" src="https://user-images.githubusercontent.com/84936545/125207770-1c06ac00-e25c-11eb-88fc-b579527e9912.png">

## How is the school summary affected?
The only school summary which was affected was Thomas High School. After removing the 9th grade scores from Thomas High School, the updated school summary data is below. 

<img width="734" alt="Screen Shot 2021-07-11 at 3 26 35 PM" src="https://user-images.githubusercontent.com/84936545/125207806-7869cb80-e25c-11eb-8fd8-4a8517d7a236.png">


### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?

When recalculating the data to find the top five and bottom five performing schools in the district, the order had not changed. Thomas High School still ranked 2nd in the district with their updated score of 90.63 overall passing %.  


Original Top 5 

![original_top_5](https://github.com/estridge2014/school_district_analysis/assets/84936545/557e9050-8f2f-4ad8-9dc2-04d84cb0dcee)

Updated Top 5

<img width="951" alt="updated top 5" src="https://user-images.githubusercontent.com/84936545/125207818-a18a5c00-e25c-11eb-90a1-cafd746616ad.png">

#### Bottom 5 

Updated Bottom 5 

<img width="951" alt="updated bottom5" src="https://user-images.githubusercontent.com/84936545/125207833-bcf56700-e25c-11eb-8253-6ba6ba7dfb4a.png">

### Math and Reading Scores By Grade

Below are the math and reading scores by grade for each individual school. 

#### Math 

<img width="350" alt="math score by grade" src="https://user-images.githubusercontent.com/84936545/125207923-66d4f380-e25d-11eb-8b94-e3074a45276f.png">

#### Reading 
<img width="350" alt="Screen Shot 2021-07-11 at 3 37 23 PM" src="https://user-images.githubusercontent.com/84936545/125208002-ecf13a00-e25d-11eb-8df9-ceca2805acd9.png">

### Scores By Spending 

Below are scores of schools based on school spending.

<img width="773" alt="average score by spending" src="https://user-images.githubusercontent.com/84936545/125208034-232eb980-e25e-11eb-95b1-23e5f311aa7a.png">


### Scores by School Type 

Below are scores of schools based on school type. 

<img width="600" alt="score by school type" src="https://user-images.githubusercontent.com/84936545/125208086-799bf800-e25e-11eb-8c43-f1088de2f44b.png">


### Score by School Size

Below are scores of schools based on school size. 

<img width="652" alt="score by school size" src="https://user-images.githubusercontent.com/84936545/125208116-a5b77900-e25e-11eb-9918-e09f441c948a.png">

## Summary 

1. In the district summary, the Percent Overall Passing Reduced by 0.3%

2. In the school summary, the Percent Overall Passing for Thomas High School reduced by 0.3%

 
After removing the testing scores of the 461 ninth graders at Thomas High School, passing percentages of the school did end up being lowered, but not by much (each less than 1%).
#### Math 

*Original: 93.27

*Updated: 93.18

#### Reading 

*Original: 97.3

*Update: 97.01

#### Overall

*Original: 90.948

*Updated: 90.63

It is difficult to come to a conclusion about academic dishonesty for Thomas High School 9th grade math and reading scores based on this analysis. When omitting the 9th grade scores, Thomas High School % passing math, % passing reading and % overall passing were reduced by <1%. This is not a large enough margin to determine academic dishonesty. Further tests will need to be implemented for a stronger conclusion.
