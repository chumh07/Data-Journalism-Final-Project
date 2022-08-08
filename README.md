# Data-Driven Story Pitch: How does Free/ Reduced School Meals affect students?
###### By Hanh Chu
## Pitch Summary 
President Joe Biden signed a new bill, the Keep Kids Fed Act, into law on June 22, 2022. This law will extend most of the federal waivers that helped millions of kids around the United States get access to meals during the school years and summer just before their expiration at the end of the month. But this new law does not extend the waiver that made all school meals free to students regardless of their family’s income. 

The National Lunch Program provides free lunch for students with a family’s income at or below 130 percent of the Federal poverty line. This still leaves students at between 130 and 185 percent of the poverty line with reduced costs of 40 cents for lunch and 30 cents for breakfast and above 185 percent with full-priced meals. These costs can add up and potentially burden families. 

I want to use data from California to explore more about the benefits of the National Lunch Program and whether or not it should expand the requirement on household income for students to receive free meals. 


## Data Visualizations 
![_Q1 Visual](https://user-images.githubusercontent.com/109722062/183426806-802f3352-1087-4ffd-8755-e56eb26b1f2f.png)


## Sources

This pitch was inspired by [this article by NBC](https://www.nbcnews.com/news/us-news/free-school-lunches-are-ending-house-passes-deal-summer-meals-child-nu-rcna34745). This project was made possible with the data from the California Department of Education's [website](https://www.cde.ca.gov/ds/sh/cw/).    

### Potential Interview Contacts
1. Ms. Cathy Ahearn 
- Email: cahearn@slcusd.org
- As a teacher working closely with second English language learners and low- income students, she understands and is familiar with the needs of the communities
- with the most participation in the National Lunch Program.

2. Ashley Salomon Gaspar
- Email: ashleyswoo@gmail.com
- She received school meals through the National School Program from K-12 and she can provide a personal experience with the pros and cons of the program. 

### Potential Additional Sources
1. [Children's Food Security and Intakes from School Meals: Final Report](https://www.ers.usda.gov/webdocs/publications/84357/ccr-61.pdf?v=4652.4)
- This study shows the relations between food security and nutrition in children in relation to school meals. 
- It could help us understand more about the role of school meals in increasing food security and daily nutrition intake across the income threshold in children. This can show how increasing the accessibility to school meals can benefit children. 

2. [The Food and Nutrition Assistance Landscape: Fiscal Year 2020 Annual Report](https://www.ers.usda.gov/webdocs/publications/101909/eib-227.pdf?v=7735.7)
- This study summarizes all of the federal programs aiming at providing food accessibility. 
- This can help understand the funding and expenses going into increasing food security across the country. We can analyze the trends and compare its effect on the well-being of children in the U.S.


## Data Analysis Process
The first step of my analysis was to clean the data using the program Refine. After inspection, I only catch some spelling errors in the school’s name and the rest of the data did not require any refining. 
The next step is to rename the data sets, bold, and freeze the heading row after uploading them onto Google Sheets. 

### Key Assumptions 
All questions were answered using the data set for the year 2020 in California from the sources mentioned above. 

### Analysis 
#### 1. What is the percentage of K- 12 students enrolling in the National School Lunch Program in each school type?

![_Q1](https://user-images.githubusercontent.com/109722062/183425284-e9eda23d-bd59-486d-a022-6af74ae642bb.png)
![_Q1](https://user-images.githubusercontent.com/109722062/183443474-2e7b9416-b097-44b1-9863-59385c5571e8.png)

##### Step-by-step answer:
1. I made a pivot table on Google Sheets
1. I set my row as school type and set my values as sum of Free or Reduced Meal Count (K-12)
1. I then copy everything except for the first row into a new sheet
1. I change the value for the pivot table to sum of Enrollment K-12
1. I copy the new column of the sum and paste it to a new column on the sheet I just created
1. I made another column and find the percentage

#### 2. Comparing the average percentage of FRPM K- 12 (Free or reduced-price meal) between charter and non-charter school
![_Q2c](https://user-images.githubusercontent.com/109722062/183422874-7b1bf961-4b5f-4ea1-86e0-751548fa6598.png)
![_Q2nc](https://user-images.githubusercontent.com/109722062/183423472-c1e06ac1-a120-4732-8500-d30086434e9b.png)
##### Step-by-step answer:
1. I put on a filter and only look at charter school
1. I highlighted the FRPM K -12 column and click on the tab at the bottom right to find the average
1. I then copy everything except for the first row into a new sheet
1. I compare the two average and non charter school (right) is higher 

#### 3. What non-traditional educational type has the lowest average percentage of FRPM K- 12 ?
![Q3](https://user-images.githubusercontent.com/109722062/183429749-5ed9c23a-97bf-462f-ba0b-edae668d06c5.png)
##### Step-by-step answer:
1. I made a pivot table on Google Sheets
1. I put educational type under filter and unselect traditional
1. I set my row as educational type and set my values as avg of FRMP(K-12)
1. I then copy everything except for the first row into a new sheet
1. I sort the column with the average from A - Z
1. Youth Authority School has the lowest average percentage of students in FRMP

#### 4. What is the number of K- 12 students that only receivied Reduced- Price Meal in each educational type ?
![Q4](https://user-images.githubusercontent.com/109722062/183432891-1aa0a2a5-d290-4eb1-804b-0a37e8fa5bf1.png)
##### Step-by-step answer:
1. I made a pivot table on Google Sheets
1. I set my row as educational type and set my values as sum of Free Meal Count(K-12)
1. I then copy everything except for the first row into a new sheet
1. I change the value for the pivot table to sum of FRMP(K-12)
1. I copy the new column of the sum and paste it to a new column on the sheet I just created
1. I made another column and subtract the free meal from the FRPM to get the answer

#### 5. How many school in each school type in Alameda county that has half or more students enrolling in FRPM K- 12 ?
![Q5](https://user-images.githubusercontent.com/109722062/183438219-ac44894b-88b0-4318-bcc7-61b663bd9526.png)
##### Step-by-step answer:
1. I made a pivot table on Google Sheets
1. I put county name under filter and unselected everything but Alameda 
2. I put percentage FRMP K-12 under filter, chose filter by condition and set it to only greater or equal to 0.5
3. I set my row as county name and add school type also as my row 
4. I then set my values as school name and change the "summarize by" tab to counta 

#### 6. How many school in each county that has less than half students enrolling in FRPM K- 12 ?
![_Q6a](https://user-images.githubusercontent.com/109722062/183441919-0ea3a536-6619-4b85-a452-a17910630544.png) 
![_Q6b](https://user-images.githubusercontent.com/109722062/183442298-f947fa72-7ae3-46b7-9c9c-9739b399d3b7.png)
##### Step-by-step answer:
1. I made a pivot table on Google Sheets
2. I put percentage FRMP K-12 under filter, chose filter by condition and set it to only less than 0.5
3. I set my row as county name
4. I then set my values as school name and change the "summarize by" tab to counta 


