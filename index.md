---
layout: default
title: Project Reflections
---

# Methodology Assignment 4

**Name:** Andrew Kim  
**UCSD email:** [akk006@ucsd.edu](mailto:akk006@ucsd.edu)  
**Section:** D42 - San Diego City & County Data Science: Permits, Citizen Services, and Flood Monitoring  
**Mentor:** Sara Agahi  
**Project:** San Diego County Weather Station Monitoring for Flood Control

**What is the most interesting topic covered in your domain this quarter?**

The topic I find most interesting is the relationship between wind patterns, terrain, and rainfall across San Diego County. Our Quarter 1 work has involved reviewing research on orographic effects and how complex terrain can influence rainfall distribution. I am interested in connecting those ideas to county weather-station observations: instead of only looking at how much rain fell, I want to understand why nearby stations might record different amounts during the same storm. This connects the physical processes discussed in the literature to our broader goal of supporting flood monitoring.

**Describe a potential investigation you would like to pursue for your Quarter 2 Project.**

I would like to investigate whether adding wind information and station characteristics improves short-term rainfall estimates compared with using recent rainfall alone. I would start with a manageable set of stations and historical storms, align their timestamps, check missing data, and confirm which wind and location variables are available. A simple persistence baseline could be compared with a regression model using recent rainfall, wind speed and direction, and elevation if available. I would evaluate prediction error on storms held out from training, including performance during heavier rainfall. The primary output would be a reproducible analysis and a website showing station comparisons and model results. If suitable water-level observations or verified flood-event records become available, I would explore their relationship to rainfall as an extension. Without those records, I would keep the conclusions focused on rainfall rather than claim to predict flooding.

**What is a potential change you'd make to the approach taken in your current Quarter 1 Project?**

One change I would make is to organize more of the analysis around individual storm events and consistent comparisons across stations. Our current work includes literature review, report development, and plans to integrate additional datasets and visualizations. I would build a shared preprocessing workflow first, documenting units, time zones, station coverage, and missing or questionable measurements. Then I would use the same storm windows for each station and compare patterns across wind conditions. This would make it easier to connect the paper replication to the county data and distinguish meaningful differences from differences caused by data quality or aggregation choices.

**What other techniques would you be interested in using in your project?**

I would be interested in geospatial visualization, lagged time-series analysis, and interpretable predictive models. A station map could help examine whether rainfall patterns vary with location and elevation. Lagged comparisons could explore whether changes in wind or rainfall at one station precede changes at another, while recognizing that correlation alone does not establish a physical cause. After establishing a simple baseline, I would try a random forest and inspect feature importance to see whether wind variables contribute useful information. I would also use validation that holds out entire storms, and potentially stations, to test how well the findings generalize. The choice of techniques would depend on the amount and quality of data we can actually obtain.
