## Instagram Profile Analysis Dashboard

### A Power BI project that analyzes one year of Instagram activity, focusing on liked content, activity patterns, followers, and following trends.

Project Overview

This project uses Instagram account data to create an interactive Power BI dashboard. The analysis focuses on three main areas:

* Posts and reels that were liked
* Accounts following the profile
* Accounts followed by the profile

The original Instagram export was cleaned and transformed in Power Query before being used in the dashboard. Only the files required for the analysis were used.

Dashboard Pages

1. Instagram Overview

Provides a general overview of Instagram activity using key metrics such as:

* Total Likes
* Total Posts
* Total Reels
* Reel Like %
* Likes by content type
* Monthly liking activity

2. Activity Analysis

Explores when liking activity occurs and helps identify activity patterns based on:

* Hour of the day
* Day of the week
* Time period: Morning, Afternoon, Evening, and Night
* Content type

The page also includes filters for date, content type, and time period.

3. Audience Analysis

Focuses on follower and following activity, including:

* Total Followers
* Total Following
* Follower/Following Ratio
* New followers by month
* Accounts followed by month

Data Model

The Power BI model contains three main fact tables:

* FactLikes — Instagram liking activity
* FactFollowers — follower activity
* FactFollowing — following activity

Supporting dimension tables include:

* DimDate — dates, months, years, weekdays, and quarters
* DimContent — categorizes liked content as Posts or Reels
* DimTime — categorizes activity as Morning, Afternoon, Evening, or Night

A separate ContentSummary calculated table is used to summarize likes by content type.

Data Preparation

The original Instagram data was provided in JSON format.

Power Query was used to:

* Import and transform the JSON files
* Convert Unix timestamps into readable dates and date-time values
* Create additional date and time fields
* Identify liked content as Posts or Reels
* Prepare separate tables for likes, followers, and following

DimDate was created using Power Query M, while ContentSummary was created using DAX.

Tools & Technologies

* Power BI Desktop
* Power Query
* DAX
* M Language
* JSON

Data Privacy

The original Instagram JSON files are not included in this repository because they contain personal account information.

The repository contains the Power BI project and project documentation without exposing the original private Instagram data.
