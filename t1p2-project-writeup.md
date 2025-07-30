---
editor_options: 
  markdown: 
    wrap: 72
---

# Team 1 Project 2 Write Up

## Running Speeds and Running Imbalance in the CU Boulder Football Team

### Member Contributions

**Ian McElveen**:

**Cecilia Gonzales**:

### Project Overview

#### Section 1: Running Speeds

**How often are athletes reaching ≥ 90% maximum velocity throughout a
training season?** 

To answer this question, we started by creating a bar
chart that displayed the count of reaching ≥ 90% maximum velocity for
each player for the training season. We defined the training season as
6/30/2024-7/1/2025. Exploring this, we found that the average times
reaching ≥ 90% maximum velocity throughout a training season for the
whole team was 11.8. We also noticed that the bar chart for the whole
team had a wide range of counts for reaching ≥ 90% maximum velocity
throughout a training season. This led us to explore bar charts on the
position level. We found that DBs had the highest average times reaching
≥ 90% maximum velocity with 18.4 and the OL had the lowest with 6.8. o
further investigate these differences, we grouped positions into broader
categories and examined their distributions. Specifically, we created
bar charts and computed averages for three main position groups:

-   Skill (DBs, WRs),
-   Bigs (OL, DL), and
-   Combo (LBs, QBs, TEs, RBs).
To no surprise, the skill group was the had the highest average (17.1), followed by 
the combo group (9.3) while the bigs had the lowest (8.9).

To better understand when players were most frequently reaching ≥ 90% of their 
maximum velocity, we created a daily summary of high-intensity efforts. We ensured
that each player's effort was only counted once per day and then counted how many
players reached this threshold on each day. We visualized the results using a line 
chart that displays the daily count of players who reached ≥ 90% maximum velocity. 
A dashed loess smoothing line was added to highlight general trends over time. This
plot allows us to see patterns in high-speed efforts across the training season—such
as whether they were clustered around specific weeks or varied steadily throughout the year.

The daily plot revealed substantial variability from one day to the next, making it 
difficult to identify clear trends across the training season. To reduce this noise 
and better observe broader patterns, we aggregated the data by week and re-analyzed 
the frequency of players reaching ≥ 90% of their maximum velocity on a weekly basis.
This data was far less noisy and allowed us to analyze the plots to determine that 
it is more common to reach ≥ 90% of their maximum velocity during the pre and post
seasons than during the actual season where games occur. On average, players reached
≥ 90% of their maximum velocity just over 31 times per week. This does not indicate 
that 31 individual players hit this threshold each week, as some players may have reached
it multiple times within the same week.

**Should we consider the number of sprinting efforts that athletes are
completing?**

**Are relative efforts and bands more advantageous than the absolute
bands provided?**

**How does sprinting exposure (# of efforts, % max reached) relate to
incidence of hamstring injuries?**

#### Section 2: Running Imbalance

**What is the variation at the team level and at each individual athlete level?**

  To understand the relationship that running imbalance has with time for the team as a whole, the average of the team's absolute value running imbalance were looked at over time. Since January 1, 2024, in general there were no large spikes in average absolute running imbalance for the team. Dates in which there is a noticeable spike are dates in which only 1 player recorded a running imbalance measurement and was therefore not indicative of the team as a whole. With this, all players in this analysis will be treated independently from one another.

  Looking ahead to see the relationship between running imbalance and HSI risk, the Running Imbalance data set was broken up into players who did and did not sustain a hamstring injury since January 1, 2024. From there, three different bootstraps were performed to understand the differences in running imbalance between the two groups.
  
  The first bootstrap was used to compare the the variance in running imbalance between the two groups, assuming that players are independent of one another. This bootstrap revealed that the group of players who sustained a hamstring injury have a greater variance in running imbalance than the group that did not sustain an injury with 90% confidence by 0.2310 to 3.4866. 
  
  Along this same thread, another bootstrap was constructed which calculated each player's variance from January 1, 2024 to the present. This means that each player had their own variance measurement and the variance wasn't calculated from the pooled bootstrap resampling algorithm. This bootstrap revealed that with 90% confidence, players who had a hamstring injury had a greater average variance than their uninjured counterparts between 0.7859 and 1.3262. This, like the last bootstrap supports the idea that players who sustained a hamstring injury have on average higher variance in their running imbalance than those who did not sustain a hamstring injury. 
  
  To understand whether or not preference for one side has a relationship with HSI risk, the third bootstrap looked at the average absolute value for each group. This bootstrap revealed that with 90% confidence the true difference in average absolute value between the groups is between 0.0535% and 0.3255%. While the difference between the two groups is statistically significant at the $\alpha$ = 0.1 significance level, the values are so small that in practice, using these values to try and differentiate the groups would be difficult considering that running imbalance ranges from 0% to 100%.
  
  This analysis also looked at the relationship that running imbalance had with the categories of positions. This analysis first looked at the average variance in running imbalance across all three categories (Bigs, Skills, and Combos) using the same bootstrapping algorithm from before. This bootstrap revealed that there was no statistically significant separation between any of the three groupings. This suggests that despite different physical demands for each position, they do not tend to vary differently from each other. 
  
  This analysis also wanted to see if there was a significant difference in the average absolute value running imbalance across the different categories. Using the same bootstrapping algorithm as before and comparing the estimated average absolute value in running imbalance for all of the categories we can see that Bigs and Combos have nearly identical estimations of the average absolute running imbalance. But, Skills actually have a significantly higher average absolute value running imbalance by about 0.2%. Again, while this is statistically significant, it's important to note that running imbalance ranges from 0% to 100% so a difference in running imbalance of 0.2% will be hard to detect in practice. This may also be just due to the different physical demands put onto Skills that are not put onto Bigs or Combos. 
  
  
**What is a meaningful change? What red flags should go off when we see a week-to-week change in running imbalance?**

  In order to see what would be a meaningful change in running imbalance, this analysis focused on what trends players had leading up to and directly following a hamstring injury. When looking at running imbalance values of players before and after an injury, there wasn't any sort of discernible trend that was applicable to most of the players. Instead what was found was that before and after a hamstring injury, running imbalance trends looked the same. 
  
  In order to further see if there is a relationship between running imbalance and HSI risk week-to-week, this analysis looked at the average running imbalance value per week leading up to and after a hamstring injury. This too revealed that there was no discernible pattern in average running imbalance value week-to-week and instances of hamstring injuries. 
  
  Finally, the same analysis was done but instead of using average running imbalance per week, the summary statistic used was variance in running imbalance per week. Like before, there was no pattern in the trends that could have been used to safely relate variance in running imbalance to HSI incidents. There was a somewhat common pattern of there being a jump in variance in the first week with data after a hamstring injury but this may be due to the fact that there is not as much data in that week and the jump in variance is due to that lack of data and how variance is calculated.
  
  We also wanted to see if there were significant detectable trends in running imbalance for athletes who sustained a hamstring injury. To see if there was, the Kendall rank correlation coefficient was calculated for all athletes with running imbalance data. These Kendall rank correlation coefficients were then put into a data set that was split into two groups, athletes who were injured and those who were not. These two data sets were then resampled 5000 times and the average absolute value Kendall rank correlation coefficient for the sample was calculated. This bootstrap revealed that there was not a statistically significant difference in Kendall rank correlation coefficient values for athletes who were injured and those who were not. In fact, the distributions for the average Kendall rank correlation coefficient values were almost identical. This implies that simply looking at trends in the data will not be indicative of whether or not a player will sustain a hamstring injury or not. 
  
  The absolute value was taken to eliminate the effect of the negative and positive Kendall rank correlation values from canceling each other out. Since a negative Kendall rank correlation values indicate a trend to prefer the left side more and a positive value indicates a growing preference for the right, using the absolute value of a trend will just indicate a growing preference toward one side.
  

**Is running imbalance sensitive enough of a metric to use as a prognosis tool versus a rehab tool?**

  To address whether or not running imbalance alone is a sensitive enough to use as a prognosis tool compared to other rehab tools, this analysis tried to look at recovery times and relate them to patterns in running imbalance. Knowing that variance in running imbalance is strongly associated with HSI risk, this analysis tried to see if variance in running imbalance was associated with a recovery time greater than what was predicted using a prognosis tool. 
  
  This analysis used the variance in running imbalance from the date of the injury to the end of the prognosis time frame given. A model was then constructed using solely the variance in running imbalance to predict whether the player returned within the predicted time frame or not. This model showed that the slope coefficient associated with variance in running imbalance was statistically significant at the $\alpha$ = 0.01 significance level and had a value of -0.04135 suggesting that a lower variance in running imbalance throughout the recovery period was associated with a higher chance of recovering within the predicted time frame. When assessing the model though, the cross validated classification error rate was 0.4. This suggests that while there is a detectable difference in running imbalance variance for players who recovered in the predicted time frame and those who did not, variance in running imbalance isn't sensitive enough of a metric to be used as a prognosis tool.
  
  To see what the relationship between variance in running imbalance and returning to play in the predicted time frame or not, another bootstrap was performed. The data was split up into those who recovered in time and those who did not. Those two data sets were then resampled 5000 times and the average player variance in running imbalance was calculated from each sample. This revealed that the players who returned to play within the predicted time frame had a lower average predicted variance in running imbalance by about 1.2 than those who did not return with in the predicted time frame. So while variance in running imbalance is not a strong predictor for whether an athlete will return to play on time on its own, it may be used to supplement prognosis estimates made using rehab tools. 


### Code Implementation

  The code for this project was designed to run sequentially. There are chunks throughout the analysis, usually at the end of each question, that remove objects from your environment that were created in the preceding analysis that are no longer needed. These were put in to increase efficiency and make it clear which objects were used for which analysis. This analysis also includes tools from the *gt*, *aod*, *lme4*, *boot*, *mgcv*, and *leaps* libraries and for someone cloning this repository, may require them to install the appropriate packages to access these libraries.

  The first section is made up of the code that reads in and cleans the three data sets that will be used for the analysis. The Catapult data set will be used to look at running speeds, the Historical Running data
set will be used for running imbalance and the Incident Report data will be used to look at injuries.

  The Catapult data set was filtered down to only include columns that had relevant statistics for the player such as their anonymous identifier and position and information about their velocities categorized through bands. The Historical Running data set only contained the anonymous ID, Date, and Running Imbalance value. So the only cleaning on this data set was to filter out rows with missing data. The Incident Report data set
was filtered down to only look at Hamstring injuries(rows where column OSICS14.Code = "TM1"). All of the data sets were also filtered down to only include data from January 1, 2024 and on.
  
  

### Final Results

#### Section 1: Running Speeds

**How often are athletes reaching ≥ 90% maximum velocity throughout a training season?**



**Should we consider the number of sprinting efforts that athletes are completing?**



**Are relative efforts and bands more advantageous than the absolute bands provided?**



**How does sprinting exposure (# of efforts, % max reached) relate to incidence of hamstring injuries?**




#### Section 2: Running Imbalance

**What is the variation at the team level and at each individual athlete level?**

  Each player tends to have a very unique variation in running imbalance. The team throughout time does not seem to have any larger spikes than normal in running imbalance suggesting that at no point in time did the team have a large shift in running imbalance all together. 
  
  Through the use of three different bootstrap algorithms, we found that players who sustained a hamstring injury have a statistically significantly higher average variance in running imbalance and average absolute value running imbalance than players who did not sustain a hamstring injury. The difference in average absolute value in running imbalance was very small though and it would be hard to differentiate the groups in practice only using the one estimated difference. 
  
  The different categories of positions tended to have the same average variance when estimated using a bootstrap method. Using the same bootstrapping method as before but estimating the average absolute value of running imbalance for each of the three categories revealed the Bigs and Combos had nearly identical estimates of the average running imbalance value of around 2.75%. But Skills had a statistically significant higher average absolute value running imbalance of around 3.15%. This may be due to the differing physical demands put onto the different categories of positions where Skills may be more inclined to favor one leg over another to accomplish their goal. 
  

**What is a meaningful change? What red flags should go off when we see a week-to-week change in running imbalance?**

  There were no discernible trends in running imbalance that were clearly indicative of an impending HSI. Instead, for players that sustained a hamstring injury since January 1, 2024, their trends in running imbalance looked almost identical before and after their injury. This supports the idea that instances of HSI aren't necessarily due to changes in running technique or side preference but instead risk is associated with someone's innate running technique. Said in other words, short term changes in running imbalance do not seem related to hamstring injuries. Instead, looking at a player's variance across their career tends to be more indicative of whether or not they would sustain a hamstring injury. 
  
  Along this same vein, players who sustained a hamstring injury and those who did not did not have a statically significant difference in Kendall rank correlation coefficients. Put simply, this means that players who sustained a hamstring injury did not have a more detectable monotonic trend (positive or negative) than their uninjured counterparts. This means that simply looking at running imbalance trends were not indicative of whether or not a player would sustain an injury. This supports the idea from before where the actual values of running imbalance are not strongly associated with injury risk, it's the variability in running imbalance that is stronger associated. 


**Is running imbalance sensitive enough of a metric to use as a prognosis tool versus a rehab tool?**

  Earlier analysis identified that variance in running imbalance across an athlete's career at CU Boulder tended to have the strongest relationship with HSI risk. For this reason, a model was built using variance in running imbalance from the date of the injury to the end of the prognosis time frame to predict whether or not the player returned to play within the predicted time frame. This model resulted in a statistically significant slope coefficient at the $\alpha$ = 0.01 significance level suggesting that there is a strong relationship between variance and the likelihood of the player returning within the predicted time frame. The value of the slope coefficient was -0.04135 which in the context of the model suggested that lower variance was associated with a higher likelihood of returning to play within the prognosis time frame. When this model was cross validated though, it had a classification error rate of 0.4 meaning that it may not be strong enough to make accurate definitive decisions about whether or not a player would return on time or not. 
  
  To see the relationship that variance in running imbalance had with return to play times, a bootstrap was performed to estimate the mean variance in running imbalance for the two groups (returned to play within the predicted time frame or not). This bootstrap revealed that players who did not return within the prognosis time frame had a higher average variance in running imbalance by 1.2 which is statistically significant at the $\alpha$ = 0.01 significance level. With there being a strong distinction between the two groups, but not enough sensitivity to make consistently accurate predictions, we suggest that variance in running imbalance throughout the recovery period could be used to supplement prognosis estimates made with rehab tools. 
  
  
### Final Results
