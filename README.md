# Kickstarting with Excel

## Overview of Project

### Purpose
Louise, an up and coming playwright, wants to create a Kickstarter campaign to provide funding for her play _Fever_. She has estimated a potential $10,000 needed to fully fund her project. The purpose of this analysis is to consider various aspects of successful and failed campaigns, in order to determine the characteristics that are correlated with each outcome, so that Louise can determine the best goal amount and timing to improve her chances of a successful campaign.

## Analysis and Challenges

### Overall Data Set Analysis
This Kickstarter dataset contains 4,114 records spanning May 17, 2009 to May 3, 2017. There are 1,393 theater projects with 1,066 within the "plays" subcategory. While there is data from as far back as 2009, the first month with more than 5 theater/play projects is not until the second quarter of 2014. 

### Analysis of Outcomes Based on Launch Date

#### Raw Total Analysis for Theater Projects
In order to provide a more robust dataset, the analysis of the outcomes based on launch date targeted the Parent Catgegory level filtered to Theater projects only. With 111 successful projects in May, and 100 successful projects in June, these far outpaced the remaining months with July as a second runner up (with 87). Early spring into summer launch dates are generally higher than the other seasons.

#### Percent of Total Success Analysis for Theater Projects
While the raw totals show a huge bias towards May and June, it is important to consider the comparison of the percent successful to failed projects to see the full picutre. According to chart 0.0 below, 10 out of 12 months had success rates over 60% with May and June coming in at 68% and 67% respectively. This suggests that while May and June were successful months, the other months of the year (except Oct and Dec) still showed a farily high success rate. 

### Analysis of Outcomes Based on Goals

#### All Outcome Analysis for Plays
In order to better understand the success rate of projects based on the Project Goals, the chart below depicts the success, failure and cancel rate for __plays__ grouped in buckets based on ranges of Project Goals. The break even point on Succssful/Falied projects falls within the 15,000 to 19,999 bucket and represents a 50% success and 50% failure rate. Project Goals below this breakpoint have a higher success rate, and projects above this breakpoint have a lower success rate.

#### Trending for Successful Play Projects
Considering there are no cancelled plays, the failure rate is an exact mirror of success rate. With this in mind, the cancelled and failed rates are unnecessary for this analysis and the charting can focus directly on Success Rate. In chart 0.0 below, a trendline shows a negative relation between goal amount and success. There is one buckt at the 40,000 level that does not conform to this trending and may represent an outlier in this data set. 

In the next visualization, chart 0.0 shows the total successes and failures within each bucket. The vast majority of the projcets fall within the first 3 or 4 bucktes, and the 40,000 buckt, which seemed to be an outlier contains only 3 total projects (2 successful) out of the 1,066 total play projects. 

The final image below (chart 0.0), shows a running total of play projects for the displayed buckets. 92% of all plays fall into the bucktes below 15,000 and 95% are below 20,000. With this in mind, the values have decreasing predictive power as the bucket values increase, due to the shrinking sample size. 

### Challenges and Difficulties Encountered
The first challenge is determining the scope of the outcome types to consider as well as pruning the data down to the apporpriate types. In my professional opinon, the analysis should be focused on completed projects. This can be overcome by removing both cancelled and live campaigns. Cancelled campaigns could be considered in a separate analysis if the dataset included some manner of cancellation category/reason. The main focus of this analsis should remian centered on a comparison of successful and failed campaigns. 
The second challenge is the wide range of project categories and subcategories. While this allows an analysis to break down and drill down to more granular comparisons, the more narrow the focus, the less predective power the smaller data set has for future campaigns as the sample size becomes smaller with each subsequent filtering. Luckliy for this analysis, the theater category represents the largest category of projects and so will suffer the least from categorical analysis. This is overcome by carefully choosing the appropriate drill level and clearly communicating it withing the charting and anlysis.
The third challenge is the lack of additional fields that could represent additional color around the reason for success or failure. Additional information like marketing budget, whether backer rewards were offerred, if the backer rewards were physical or not, and whether the leader or group creating the project have had a successful campaign previously would all help provide a more comprehensive analysis. This cannont be overcome with the current data set, but could be overcome by checking the source data for additional fields.

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
1. May appears to have the highest correlation with Theater project success with 111 successful and a 68% success rate.
2. December is the worst launch month, with successful and failed projects almost equal. There were only 37 successful projects with a 51% success rate.

- What can you conclude about the Outcomes based on Goals?
1. The success rate has a negative correlation with goal amount. The higher the goal set, the lower the success rate.
2. Setting a goal less than 15,000 would provide more than a 50% chance to succeed with an even better chance of success if the goal is set less than 10,000. Considering the estimate of 10,000, there would be a greater chance of succeeding by setting a goal lower than 10,000 and making up the difference in another way (e.g. Corporate Sponserships or Advertising).

- What are some limitations of this dataset?
1. The dataset is sparse for projects before 2014 and only four full months provided in 2017
2. There are no explanations for success, failure, or cancellations
3. There is no listing of the author or organization that created the campaign, so there can be no analysis of if that group has had previous success
4. This dataset is in multiple currency types. This needs to be converted to one standard currency for a standard analysis.

- What are some other possible tables and/or graphs that we could create?
1. Charting/Analysis of the lenght of campaigns (Are longer campaigns more or less successful?)
2. Charting/Analysis on Spotlight. (Are projects listed as a Spotlight more successful?) 
3. Charting/Analysis on _nearly_ successful campaigns (How close were failed camaigns to be successfully funded?)
