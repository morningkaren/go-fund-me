# go-fund-me
Linear Regression Project

The purpose of my project called Go Fund Me is to predict the percent of goal a person is expected to fundraise given 
certain characteristics of his or her campaign on the crowdfunding platform, Go Fund Me. This was the first project
I used web scraping techniques on.

Since I wanted to predict how much I could fundraise from the beginning of a campaign, there were only certain data 
I could use, such as the description of the campaign, the goal amount, and the category of the campaign. With the campaign
description, I generated the word count, polarity and subjectivity scores. My data also had weird outliers, such as people
whose campaign goals were $1, campaigns that have surpassed their goals over 100 fold, and campaign descriptions that were 
8 words long. I dealt with some outliers by limiting my target from 0 to 1, so campaigns that reached more than 100% of
their goal was reduced to 100% of their goal. The key assumption I made, which skewed my results was that the campaigns
were finished when I scraped my data. I did not take time into consideration. 

Although that assumption was the flaw in my project, I still found some interesting results using linear regression
techniques.  I got an R^2 score of around .42, which was not bad but wasn’t great. I was essentially predicting human 
behavior which is very difficult. But, the interesting part is the relationship between the categories of campaigns and
the percent boost or percent reduction in their goal achieved. Campaigns that were for weddings received about a 20  percent
reduction on average in their goal achieved and campaigns for medical reasons received about a 40 percent boost on average 
in their goal achieved. Category alone tells you a lot about how much of your goal you may be able to obtain. 

