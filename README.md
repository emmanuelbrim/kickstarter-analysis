# AN ANALYSIS OF KICKSTARTER CAMPAIGNS 
**Analyzing Kickstarter Data to Gain Insight Into Their Outcomes.

## Overview of The Project

Crowdfunding projects can be sucessful or fail. What informs thier final outcomes is key to future exercises.
This project invloved the use of Excel to analyze data from crowdfunding projects in 21 countries to unravel possible key indicators that contributed to their outcomes.
The information revealed from the analysis of the data is narrowed down to provide insight into why crowdfundraising campaigns for some theatre productions succeeded whiles others failed.

### Purpose
The purpose of this project is to help Louise, a playwright make informed decision on kickstarting her play "Fever". The intent is to analyze data from other campaigns in order to provide louise with information on the relationship that exist between lunch dates or funding goals and the final outcome of these campaigns. 

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date

An analysis of the time a campaign was lunched in relation to its outcome provided interesting information.
Since the focus of here is on outcomes for theatre productions based on lunch dates, it was prudent to convert the Unix Timestamps to readable forms so that the year of the campaigns could be generated. Separate columns(Q and R) were created on the kickstarter sheet to hold date created conversion and Years data respectively.
Then a pivot table was created using data populated from the original Kickstarter data set to identify trends. The table included all outcomes in column "F" (not including live) marched against the lunch dates of all campaigns in column "R". This invloved selecting lunch dates as the Axis for the table and outcomes for the series and value area of the table. The enitre table was filtered by Years and Parent catergory to reflect different trend at each period. 
In the final analysis of the data on lunched dates, a line chart was created to represent the outcome of all theatre funding campaigns based on their launch dates.

The chart below shows the relationship between launch dates and outcomes of crowdfunding campaigns for theatre.
https://github.com/emmanuelbrim/kickstarter-analysis/commit/a8a12e39f1f12a25df0f50fe2bc8adf328135934#diff-d9373ec0288fcac90082d42bde8a1a3bd5b3274af45eec0958eae78884c77222

### Analysis of Outcomes Based on Goals
One of the questions that louise sort to get an answer to was if an outcome of a kickstarter campaign is influenced by the funding goal.
In order to provide this, a new worksheet was created with column headers for all Funding Goals, their outcomes,ie successful, failed and canceled and their percentages. 
In the "Goal" column, all the goals of kickstarter campaigns were categorized based on a 5000 amount range. The COUNTIFS function was then used to populate the number of outcome from each range in the Goal column "A" using "play" a subcategory of theatre. The result was the number of successful, failed and canceled outcomes for each range of funding goal shown in column B, C and D. To generate a more refined result, the percentages of each outcome was created in column F, G and H by dividing the values in B, C and D by the total outcomes in E and changing the number format to percentages.
In the end a line chart was drawn to show outcomes based on goals with funding goals and percentages of each outcome as its fields. 
Below is a line chart showing the relationship between funding goals and outcomes.
![Outcomes vs Goals](path/to/Outcomes_vs_Goals1.png)

### Challenges of The Project
Though the data set includes facts about kickstarter campaigns, the analysis that was carriedout in this project was focused on a single category; theatre.
The analyst must therefore remember to always filter his source data to reflect this area of enquiry. 
On the horizontal axis of the line chart "Outcomes_vs_Goals" holds the amount ranges for all the funding goals. However the values could only fit after font size was reduced which made its data point difficult to read. A Line chart with markers is therefore more appropriate to represent such information.  

## Results
- The most successful kickstarter campaigns for theatre was launched in May and the month of october recorded the highest in failed campaigns.
- Kickstarter Campaigns with goals of an amount lessthan 5000 were more successful.
- Though the analysis shows that goals within reasonable amounts are more successful, it is equally important to know what motivates backers of such goals.
- Histogram and bar charts


