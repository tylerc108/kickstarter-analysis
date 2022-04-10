# Kickstarting with Excel

## Overview of project
### Purpose
For this project, we analyzed a data set containing information regarding fundraising campaigns that were run using the crowdfunding platform, _Kickstarter_. We are helping our friend, Louise, who is trying to run her own fundraising campaign in an effort to put on a play, titled _Fever_. Before beginning her campaign, she wanted to analyze data collected on thousands of other fundraising campaigns to see if she could find any insights on which campaigns are successful or not successful, and why some campaigns raise more funding than others. Using these insights, Louise can further increase the chances of her fundraising goals being reached and her play being successful.

## Analysis and Challenges
### Analysis of Outcomes Based on Launch Date
In this part of our analysis, we looked into how the time of year effected the outcomes of the campaigns. This is very useful information for Louise to know, because if there is any correlation between the time of year the campaigns were launched and the success rate, she can aim to launch her campaign in the time of year when success rates were the highest. This could potentially increase her chances of her campaign being successful. We developed a pivot table to display data based on outcomes in each month of the year. There were four possible outcomes for a campaign in the data we had; these included "canceled," "live," "failed," and "successful." . We used the YEAR() function in Excel to create a column displaying year of each launch date so that we could filter based on year if necessary. Our pivot table can be seen below:

<img width="347" alt="Screen Shot 2022-04-10 at 3 22 19 PM" src="https://user-images.githubusercontent.com/103055666/162636223-6bba962c-a3f3-422d-b444-9476a5513ad6.png">

In order to map and visualize the data in a more easily understood fashion, we also created a line graph using data from the pivot table. The graph is displayed below:

  ![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/103055666/162633724-310f1790-0d15-4305-bfc9-4da48c36954f.png)

As you can see in this graph, the frequency of "canceled" outcomes remained extremely constant throughout each month. To a lesser degree, this was also true for the frequency of "failed" outcomes. The number of failed outcomes fluctuated somewhat, and seemed to slightly increase in the summer months and the month of October, but still remained mostly constant throughout the year. The frequency of "successful" outcomes, however, did appear to display a correlation with time of year. There is a very clear spike in successful campaigns that starts in late spring and continues through the summer months. The rate od successful campaigns significantly decreases once the summer months transition into the fall months.

### Analysis of Outcomes Based on Goals
This portion of our analysis focuses on how the fundraising goal set at the start of each campaign affected each campaign's outcome, focusing on the campaigns that were in the "plays" subcategory. This information would also be useful for Louise to know, so she can see if the goal she sets is likely to be reached based on outcomes of past campaigns. This would allow her to tailor her campaign goal and therefore increase the chances of her campaign being successful. To conduct this analysis, we developed a table on which to display the data we need for this analysis in a separate sheet. We used a few formulas to gather the data into this table from the "Kickstarter" sheet. First, we used the =COUNTIFS() function to gather the number of campaigns of each outcome in the "plays" subcategory and then categorized them based on the goal set at the start of the campaign. We then used the =SUM() category to find the total number of campaigns in each goal category. Finally, we calculated the percentage of each outcome within each goal categorie we created. The finished table can be seen here:

<img width="751" alt="Screen Shot 2022-04-10 at 3 37 41 PM" src="https://user-images.githubusercontent.com/103055666/162636681-50c0889f-1088-49a1-9c6c-3903a56cecff.png">

From there, we created a line graph that would better map out the relationship between the campaign goal and the outcome of the campaign. Our graph for this portion is displayed in the chart below:

![Outcomes_vs_Goals](https://user-images.githubusercontent.com/103055666/162634832-92f2ef08-33c5-4ff4-a82b-c9c9ea89159d.png)

### Challenges and Difficulties Encountered

A big challenge in this analysis was finding a correlation between outcomes and goals. The analysis we conducted for the relationship bewtween outcomes and launch dates yielded a fairly straightforward conclusion, that outcomes were best in the summer. However, for the next portion of the analysis, it was a little bit more difficult to find a relationship between our two variables. The outcomes seem to get worse as the goals increase, but it is difficult to outright declare this correlation because there is a very big exception in that the goal categories "35,000-39,999" and "40,000-44,999" defy this correlation. To overcome this challenge, we can note this exception in our conclusion as well as take note to conduct further analysis focused on these two goal categories and their percentage of successful outcomes in the future.

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

Based on our analysis, we can conclude that outcomes for theater campaigns are best in the late spring and early summer months. Conversely, we can conclude that success rates are worst in the winter months. These two conclusions lead us to recommend that Louise launch her campaign around the start of summer, ideally in May or June. Another conclusion we can draw is that the time of year did not have much if any effect on the number of canceled campaigns.

- What can you conclude about the Outcomes based on Goals?

With the exception of the goal categories "35,000-39,999" and "40,000-44,999," it seems that the higher the goal was the lower the percentage of successful outcomes became. Those two exception categories could potentially be a "sweet-spot" where success rates are good and fundraising goal is high, and Louise may be best off setting her goal in one of those two categories because they are high fundraising goals with high percentages of success based off our analysis of this data. Interesting to note is that there were no canceled outcomes in this data set, i.e. no campaigns in the subcategory of "plays" were canceled. 

- What are some limitations of this dataset?

As with any data set, this is data set has a limited sample size and doesn't include every single fundraising campaign ever conducted. It only includes those run on the platform _Kickstarter_, and there are many other crowdfunding platforms that have been used to run fundraising campaigns. It would be useful for future analysis to look into fundraising campaing platforms other than _Kickstarter_ to further grow the scope of our analysis. This datset also doesn't include fundraising campaigns that were run without the use of an online fundraising platform at all, and this may be something that could be useful to look into in future analysis.

- What are some other possible tables and/or graphs that we could create?

Because there are many more variables that could affect outcome in this dataset other than the ones we analysed, there are many other graphs and tables we could create. We could create a table and line graph that displays percentage of outcomes based on average donation, for example, or a table and stacked bar graph that displays percentage outcomes based on country.
