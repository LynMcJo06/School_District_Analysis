# School_District_Analysis
Module 4 Pandas the work will be completed using this repo.  
##  Module 4 Course Work
  Maria is a Chief Data Scientist for a city school district.  She is responsible for preparing all standardize test data for analysis, reporting and presentation.  This data will be used to provide insights into performance trends and patterns.  Our role is to assist Maria analyze data on student funding and student's standardized test scores.  We will be showcasing trends in school performance.  The school board and superintendent will use the information in making decisions on school budgets and priorities.  The data is highly confidential and must be protected.  
  We are fairly new team members, so we leaned heavily on Maria for assistance.  We installed Anaconda as our analysis will be conducted using Python and Jupyter Notebook.   
We started by creating a development or virtual environment and a clone of the GitHub repository to be consistent and to interact with the other team members.   
We converted the Excel file to a Pandas DataFrame.  Maria advised us that the team uses Jupyter Notebook for the analysis; therefore, we familarized with this tool.  The most helpful item we learned about was creating and using DataFrames in Jupyter Notebook.  Maria shared CSV format datasets that we imported and reviewed.  Anomalies were noted while reviewing the CSV files.  After starting our first notebook and importing the data files, we committed our work to GitHub via GitBash.  The learning never ends.  
  In Lesson 5, our job was to clean the data prior to performing any analysis.  We learned how to check for missing data, and were thrilled to find that our CSV files did not have any missing data.  Maria, being the thorough teacher, gave us a file that did have some missing so we could practice.  After practicing with the missing data files, we retuned to our school district analysis.  We checked that the data in each column was in the correct formate for us to conduct our analysis.  One major issue with the student dataset was that some names had professional prefixes and suffixes.  We knew this could not be correct as our dataset involed high school students.  It took several steps and differnt functions to remove the unwanted prefixes and suffixes, but the data looked great afterwards.  The two separate dataframes were merged as our analysis would involve gleaning information from the whole district.  
  In Lesson 7, we started consolidating information to assist with the analysis.  We needed to get the following information:  
  * total number of students
  * total number of schools
  * calculate the total budget for the district
  * average math scores
  * average reading scores
  * student passing math percentages
  * student passing reading percentages
  * student overall passing percentages

After gathering and calculating this information, we created a District Summary dataframe that would enable Maria to pass the information to the stakeholders.  It was important that the data within this dataframe be in the proper reporting formats.  This completed this portion of our analysis.  
'-----
After our marvelous work with the district summary, Maria wanted us to create a similar summary for each school.  We got to work.  Our dataframe included school type, total budget, budget per student, average math and reading scores, math and reading passing percentage, and the overall passing percentage for each school.  From this analysis, we determined the highest-performing schools based on the overall student passing percentage.  The top five performing schools were all charter schools with overall budgets around $1,000,000 with the exception of Wilson High School and Pena High School, whose bugets were $1.3 million and approximately $600,000, respectively.  The top five school's student population ranged from approximately 1,000 to 2,200 students.  The overall passing percentage for each of the top five schools was 90% or better.  
The lowest performing schools were district schools with overall budgets ranging from $1.8 to 3.1 million.  In contrast to the top five schools, the lowest five schools had student populations ranging from approximately 3,000 to 4,800 students and overall passing percentages around 53%.  
'-----
In Lesson 11, we established spending ranges per student, categorized the spending bins, grouped the data by the spending ranges and created a new DataFrame for the scores by school spending.  Our original breakdown of the spending bins had to be adjusted as the schools were not fairly grouped.  I was surprised by the results of the analysis:  the schools with the smallest per student spending had the highest Average and Percent Passing Math and Reading Scores, and the highest overall percentage passing.  
'-----
In Lesson 12, we grouped the averages and percentages by school size as Maria was curious if size had an impact on math and reading scores.  We created three bins, small, medium and large, for the school bins.  After created the three bins, we grouped the schools into the bins and added the results to our existing school summary.  Once again, we grouped the average math and reading scores, the average percentage passing math and reading, and the overall passing percentage based on school size.  The results of this analysis showed that attending a small to medium sized school produced higher scores and percentages.  The difference in overall percentage passing was shocking:  both small and medium size schools were 90% or better; the large schools dropped to 58%.  
'-----
For our final analysis, Lesson 13, we grouped the average passing scores and percentages in math and reading, and the overall percentage passing scores by school type.  Once again, insightful information.  It is beneficial to be a student at a charter school as the scores and percentages are higher.  
From this analysis, one can conclude that the smaller the student population size, the more likely each student is to succeed.  

## Module 4 Challenge
### Overview
The school board notified our department that there is evidence of academic dishonesty with the math and reading grades for the ninth graders at Thomas High School.  In order to meet state testing standards, the school board has asked our department for assistance in addressing this academic dishonesty.  During an internal staff meeting, we decided to replace all the Thomas High School ("THS") ninth grade math and reading scores with NaNs or "not a number", which should address any disparity created by the academic dishonesty.  We decided that replacing this data would be our best option.  THS data for grades 10th, 11th, and 12th appeared to be academically sound.  Additionally, THS budget, size, and type were critical to our overall analysis.  We repeated the school district analysis with the excluded THS ninth grade math and reading scores eliminated from the calculations.  The following sections address the results of this modified analysis.  
### Results
After reviewing the results of the analysis conducted after eliminating the THS ninth-grade, grade data, the following observations were made:  
  - In the District Summary, the Average Math Score, Average Read Score, Percent Passing Math, Percent Passing Reading, and the Percent Overall Passing, were 78.9, 81.9, 74.8%, 85.7%, and 64.9%, respectively.  These totals equated to a slight decrease from the original District Summary figures as follows.  
     - The change in the Average Math Score was approximately 0.13% lower
     - The change in the Average Reading Score did not change
     - The change in the Percent Passing Math was approximately 0.27% lower
     - The change in the Percent Passing Reading was approximatly 0.33% lower
     - The change in the Percent Overall Passing was approximately 0.46% lower
  - The school summary was only slightly different after the THS ninth grader scores were eliminated from the analysis.  
  -   - The change in the Average Math Score was approximately 0.05% lower
  -   - The change in the Average Reading Score was approximately 0.05% higher
  -   - The change in the Percent Passing Math was approximately 0.02% lower
  -   - The change in the Percent Passing Reading was approximately 0.30% lower
  -   - The change in the Percent Overall Passing was approximately 0.33% lower
  - Replacing the ninth graders' math and reading scores did not affect THS's performance relative to the other schools.  THS was still the second highest ranking school behind Cabrera High School in both analyses.  Consistent with the previously-mentioned results for the District and the school summaries, the changes were less than 0.5%.  
Additional comparison was conducted as follows:  
  - 
 

I was expecting a greater change in the data as a result of eliminating the THS ninth-grade, grade data.  
