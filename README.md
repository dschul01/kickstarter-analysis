# An Analysis of Kickstarter Campaigns
Performing analysis on Kickstarter data to uncover trends driving the success of campaigns.
## Overview of Project
### Purpose
The client, Louise, began a Kickstarter campaign with a goal of $10,000 to fund her play, “Fever”, and was close to meeting the goal in a short amount of time.  She is interested in the success rates for Kickstarter campaigns and would like to understand how funding goals and launch dates impact them.  The purpose of the project is to utilize Excel to determine the success rates based on factors including launch dates, funding goals, as well as type and location.  The project analyzed > 4,000 campaigns across multiple categories and countries from 2009 – 2017 to provide guidance on success.
## Analysis and Challenges
### Analysis of Outcomes Based on Launch Date
The original Kickstarter campaign data was utilized to determine if the launch month impacts success.  An additional column was created within the original “Kickstarter” sheet to provide the ability to look at individual years to determine if YoY trends exist.  A pivot table was created to summarize outcome of campaigns based on category and launch month with a filter for “Campaign Category” and “Year”.   Since the purpose is to analyze results of campaigns that have ended, the pivot table was filtered further to remove volumes of “live” campaigns.  

The pivot table was utilized to create the line chart below to illustrate the campaign outcomes based on launch date of theater campaigns.  Observations of the data follows:
* More successful campaigns started between the months of May through July although volumes decrease almost every month after the May peak.  
* Failed campaigns follow a similar trendline as successful campaigns but not to the same degree.
* Canceled campaigns are flat indicating campaign start does not influence this outcome.
* Decisive evidence correlating campaign start month to outcome can not be made from this chart alone 
 
Conclusions and limitations are discussed later in this evaluation.

![Theater_Outcomes_vs_Launch](https://github.com/dschul01/kickstarter-analysis/blob/main/Resources/Theater_Outcomes_vs_Launch.png)

### Analysis of Outcomes Based on Goals 
The original Kickstarter campaign data was utilized to analyze the percentage of success based on goal ranges.  Goal ranges were established and then ‘countifs’ formulas were utilized to obtain the campaign volumes by outcome.  Percentages of campaigns by the range amounts were calculated using the outcome volumes. 

The resulting calculations were used to create the line chart below to illustrate the campaign outcomes based on goal ranges.  Observations of the data follows:
* Campaigns are more successful when they are either below $15k or between $35k and $45k.
* Campaigns start to fail more often between the goal ranges of $15k - $35K
* Campaigns were almost certain to fail once they reach $45k

Conclusions and limitations are discussed later in this evaluation.

![Outcomes_vs_Goals.png](https://github.com/dschul01/kickstarter-analysis/blob/main/Resources/Outcomes_vs_Goals.png)

### Challenges and Difficulties Encountered
The main challenge I encountered is the lack of detailed information on the campaigns in order to provide better analysis.  Additionally, there is a need for data on donation trends and other crowdfunding sites to form a more educated decision.  

## Results
### Conclusions
Two of the conclusions which can be formed as a result of data from "Outcomes based on Launch Date" are:
1. Launching a theater campaign in May brings the highest success rate.
2. Launching a theater campaign in December brings the highest failure rate.

One conclusion which can be made as a result of data from “Outcomes based on Goals” is that a theater campaign has the highest percent of success if the campaign is less than $1,000.  There is still high probability up to $5k, but then declines from there until an anomaly within the $35k to $45K goal range.

### Limitations of the Dataset

The current dataset is limited in its details, amount of data, and info on those who have funded campaigns.  There are many data elements which would be helpful in providing more conclusive analysis on the kickstarter data.  Breaking down plays by genre, narrowing the location of the campaign, and adding in additional crowdfunding sources would be a start.  Additionally, obtaining demographic information for those who have funded campaigns would also be useful.


Another table I recommend creating would be combining the result of the timing of the campaigns along with the goal ranges.  This would allow us to determine best time to start campaigns of different goal magnitudes. 
