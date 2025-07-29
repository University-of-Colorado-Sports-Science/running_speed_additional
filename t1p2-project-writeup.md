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

**What is the variation at the team level and at each individual athlete
level?**

To understand the relationship that running imbalance has with time for
the team as a whole, the average of the team's absolute value running
imbalance were looked at over time. Since January 1, 2024, in general
there were no large spikes in average absolute running imbalance for the
team. Dates in which there is a noticeable spike are dates in which only
1 player recorded a running imbalance measurement and was therefore not
indicative of the team as a whole. With this, all players in this
analysis will be treated independently from one another.

Looking ahead to see the relationship between running imbalance and HSI
risk, the Running Imbalance data set was broken up into players who did
and did not sustain a hamstring injury since January 1, 2024. From
there, three different bootstraps were performed to understand the
differences in running imbalance between the two groups.

The first bootstrap was used to compare the the variance in running
imbalance between the two groups, assuming that players are independent
of one another. This bootstrap revealed that the group of players who
sustained a hamstring injury have a greater variance in running
imbalance than the group that did not sustain an injury with 90%
confidence by 0.2310 to 3.4866.

Along this same thread, another bootstrap was constructed which
calculated each player's variance from January 1, 2024 to the present.
This means that each player had their own variance measurement and the
variance wasn't calculated from the pooled bootstrap resampling
algorithm. This bootstrap revealed that with 90% confidence, players who
had a hamstring injury had a greater average variance than their
uninjured counterparts between 0.7859 and 1.3262. This, like the last
bootstrap supports the idea that players who sustained a hamstring
injury have on average higher variance in their running imbalance.

To understand whether or not preference for one side has a relationship
with HSI risk, the third bootstrap looked at the average absolute value
for each group. This bootstrap revealed that with 90% confidence the
true difference in average absolute value between the groups is between
0.0535% and 0.3255%. While the difference between the two groups is
statistically significant at the $\alpha=0.1$ significance level, the
values are so small that in practice, using these values to try and
differentiate the groups would be difficult considering that running
imbalance ranges from 0% to 100%.

**What is a meaningful change? What red flags should go off when we see
a week-to-week change in running imbalance?**

**Is running imbalance sensitive enough of a metric to use as a
prognosis tool versus a rehab tool?**

### Code Implementation

The code for this project was designed to run sequentially. There are
chunks throughout the analysis, usually at the end of each question,
that remove objects from your environment that were created in the
preceding analysis that are no longer needed. These were put in to
increase efficiency and make it clear which objects were used for which
analysis. This analysis also includes tools from the *gt*, *aod*,
*lme4*, *boot*, *mgcv*, and *leaps* libraries and for someone cloning
this repository, may require them to install the appropriate packages to
access these libraries.

The first section is made up of the code that reads in and cleans the
three data sets that will be used for the analysis. The Catapult data
set will be used to look at running speeds, the Historical Running data
set will be used for running imbalance and the Incident Report data will
be used to look at injuries.

The Catapult data set was filtered down to only include columns that had
relevant statistics for the player such as their anonymous identifier
and position and information about their velocities categorized through
bands. The Historical Running data set only contained the anonymous ID,
Date, and Running Imbalance value. So the only cleaning on this data set
was to filter out rows with missing data. The Incident Report data set
was filtered down to only look at Hamstring injuries(rows where column
"OSICS14.Code" = "TM1"). All of the data sets were also filtered down to
only include data from January 1, 2024 and on.

### Final Results
