# An Analysis of kickstarter Campaigns

## Kickstarter data analysis

Use excel to find Trends and Patterns:

* Formating, filtering,  the data for initial data exploration and analysis - See Kickstarter worksheet
 
* Create new variables (Columns) and Debugging using excel formulas: See Kickstarter worksheet

_ _  Percentage Funded, Average Donation, Parent Category, Subcategory
_ _  Date Created Conversion, Date Ended Conversion by converting Unix Timestamps to Readable Format

* Creating Pivot Tables and Charts - See Workbook data 1-1-3-StarterBook:
_ _ Category Statistics, Subcategory Statistics, Outcomes Based on Launch Date

* Box-Plots and a Five-Number Summary (i.e. The minimum, Q1 (the first quartile), the median, Q3 (the third quartile), the maximum) - See Box Plots worksheet
 
### Results Summary 
* The disrtibutions of the Campaign Goals and the Amount Pledged are not normal, and as it is seen in the plot box bellow the data is highly skewed to the right i.e. some large values are impacting these distributions. The data has outliers, therefore for any further analysis ths should be taken into consideration. For example, instead of using the mean, it will be more appropriate to use the median as measure of Central Tendency.
* 
![Campaign Goals Distribution vs Total Amount Pledged Distribution](https://user-images.githubusercontent.com/34750363/147622525-84e1f8b5-8918-490f-be3b-a8c32a94a94e.png)
* The succesful goals were for much smaller amount of money compared to the failed goals.

![Comparison between goals and pledges distribution](https://user-images.githubusercontent.com/34750363/147623354-475fd2b4-aacf-45b4-8c52-0a56778668e8.png)

* The theater parent category outcomes in the plays subcategories were the most successful campaigns

![Parent Category Outcomes Graph](https://user-images.githubusercontent.com/34750363/147616472-5ff084bf-1be5-471e-972c-5db383d942f0.png)

![Subcategory Outcomes Graph](https://user-images.githubusercontent.com/34750363/147616483-cc108046-a7d1-4d71-b8ca-8617567646f0.png)

* Months of May and June were the most successful in for the campaigns - See Outcomes Based on Launch Date pivot chart

* _ _ See the chart below:
![Outcomes Based on Launch Date Graph](https://user-images.githubusercontent.com/34750363/147601746-001417e3-8206-407d-9632-6ef3ab33c9e4.png)

<p>&nbsp;</p> <!-- Adding a blank line -->

# Kickstarting with Excel

## Overview of Project
   Our client’s Fever play fundraising ended nearly reaching its goal within a short time. Now, the client would like to know how different campaigns performed in relation to      their launching dates and their funding goals.
### Purpose
   Use excel, and the Kickstarter dataset to analyze and visualize campaign outcomes based on their launch dates and funding goals. Then, draw a conclusion based on analysis        findings.
## Analysis and Challenges
      
### Analysis of Outcomes Based on Launch Date
    -	Created a new column named "Years" in the Kickstarter dataset using excel YEAR function to extract years from the “Date Created Conversion” column. 
    -	Created an excel pivot table from the Kickstarter worksheet and moved it in a new worksheet that I labeled “Theater Outcomes by Launch Date."
    -	Filtered the pivot table according to "Parent Category" and "Years” and placed the appropriate pivot table fields in the columns (i.e. outcomes), rows (i.e. Date Created         Conversion), and values (i.e. outcomes)
    -	Filtered the column labels to show only "successful," "failed," and "canceled."
    -	Filtered the “parent category” to show only data for “theater.” Then, sorted the outcome campaigns in descending order.
    -	Finally, I create a line chart (i.e. Theater outcomes based on Launch Date) from the pivot table to visualize the relationship between outcomes and launch month. 
  
![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/34750363/148093537-752d061c-632b-4750-8b77-ea38518bb75a.png)
<p>&nbsp;</p> <!-- Adding a blank line -->
### Analysis of Outcomes Based on Goals
    -	Created a new worksheet “Outcomes Based on Goals” in the Kickstarter_Challenge workbook
    -	Created eight columns in the new sheet (i.e. goal, number successful, number failed, number cancelled, total projects, percentage successful, percentage failed, percentage       cancelled.)
    -	Created a dollar-amount ranges in the “Goal” column so projects can be grouped based on their goal amount.
    -	Used COUNTIFS() excel function and the dollar-amount ranges in the “Goal” column to populate number successful, number failed, number cancelled columns
    -	Used SUM() excel function to populate  the project total column
    -	 Calculated the percentages using values in a  of number successful, number failed, number cancelled columns divided by a row total project value
    -	Finally, I created a line chart titled "Outcomes Based on Goal" to visualize the relationship between the goal-amount ranges on the x-axis and the percentage of                 successful, failed, or canceled projects on the y-axis.
 
![Outcomes_vs_Goals](https://user-images.githubusercontent.com/34750363/148093740-7abff505-acf1-4b32-9337-8dfb2c9c16e8.png)
<p>&nbsp;</p> <!-- Adding a blank line -->
### Challenges and Difficulties Encountered

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
<p>&nbsp;</p> <!-- Adding a blank line -->
May was the successful month for our client campaign, while May and October were the most unsuccessful months for the campaign. For the cancelled campaigns, January was the highest while, for other months appear to have the same outcomes except October where there was no outcome cancelled.
<p>&nbsp;</p> <!-- Adding a blank line -->
- What can you conclude about the Outcomes based on Goals?
The campaigns were most successful for the amount $5000, and the most unsuccessful were the campaigns above $45000. For the canceled campaign there were no peculiar month for the cancelation.
<p>&nbsp;</p> <!-- Adding a blank line -->
My conclusion is that the fund raising campaigns are more successful for small goals (i.e. less than $5000)
<p>&nbsp;</p> <!-- Adding a blank line -->
- What are some limitations of this dataset?
<p>&nbsp;</p> <!-- Adding a blank line -->
This dataset could be more useful, if it could show the backgroung of the pledging individuals or entities (i.e. participants background). Because, our client could run a more targeted fund raising campaigns.
<p>&nbsp;</p> <!-- Adding a blank line -->
- What are some other possible tables and/or graphs that we could create?
<p>&nbsp;</p> <!-- Adding a blank line -->
 We could run category and subcategory statistics tables, and outcomes based on goals by country tables.
