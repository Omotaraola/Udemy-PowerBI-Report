# Udemy-Analysis

I joined a 30 days data challenge in November 2022 and this Udemy courses dataset was part of the dataset for practice, used excel for cleaning and pivot table for visualization then. Understanding PowerBI skill better, decided to visualize this dataset again on Power BI.

## Introduction

This dataset consists of courses Udemy offered 2011 up to the year 2017, it consists of four (4) courses data table (Graphic Design, Musical Instrument, Web Development and Business Finance). Across these four data tables, they all have 12 columns and the same column titles (course_id, course_title, Url, price, num_subcribers, num_reviews, num_lectures, level, rating, content_duration, published_timestamp and subject).

## Report Objective

- To know total subscribers over the years and what year had the highest subscribers.
- What course generated the highest profit from 2011 – 2017.
- What year had the highest profit and why.

## Data Tools Used 
Microsoft Power BI

## Data Cleaning

First process I did, was append the data tables to a single table, this is to make the cleaning process faster.

![](Appending%20process.png)

This changed brought mixtures of courses in the subject column, unlike before where it had a specific course on separate data table. 

![](Appended%20table.png)

Thereafter, I observed the Url column which consists of the links that contains the course title. Having the course title in place, the Url is removed. 

![](URl%20removal.png)

The published_timestamp, has both date and time data type, changed it to only date. Then proceeded to make the date in ascending order, this is to have the older dates first before the recent dates. 

An Amazing part of using power query that save time, is the data profiling. The column quality, distribution and profile, these tools makes data cleaning easy and faster, giving columns summary.

![](Column%20Profile.png)

The column profile for course_id, indicates 2 Id’s with duplicate values all through the other columns,checked for it, and sorted them. They had the same values all through the other columns, having a diffrence of a letter, causing a mispelling in the course title column and this resulted to duplicates. This is removed thus making the data clean with no duplicates. 

Changed the price data type to currency.

Changed the Letter case of course_id, course_title, level, and subject columns, from a Lower case to upper case. Renamed the column num_subscribers to Total_subscribers, num_reviews to Total_reviews, num_lectures to Total_lectures, content_duration to Course_duration, published_timestamp to Date, and price to Course_fee,while the Rating column maintains its upper case. 

Further Checked for missing or null values and there are no null /missing values.

## Report Visualization Using Power BI

![](PowerBI%20Dashboard.png)

According to this Report Objective;

- To know total subscribers over the years and what year had the highest subscribers.

The Total Subscribers from 2011- 2017 is 12 million. Every year Udemy has new subscribers, as at 2014, Udemy had 4 million subscribers, but for the year 2015, there was a massive increase of additional 4million subscribers. This could be as a result additional Web development and business finance courses that was provided. 

![](2014%20Subcribers.png)                                      ![](2015%20Subcribers.png)


- What course generated the highest profit from 2011 – 2017.

According to the Report, Web development has always been trending financially, except for the 2014, where Business finance was topping the finance against Web development  with very little difference. 

- What year had the highest profit and why.

The year 2016 had the highest profit with a margin of $16,335 from the previous year. This could be the effect of increase in subscribers and some course fee of some subject such as Web development and Business finance.

## Conclusion

Courses such as Web development and business finance are constantly on the top chart of the finance. The world is evolving and as such many businesses will be created, and younger generations wants to be advanced in technology. It is advisable that Udemy Provide more courses in these subjects in better standards, this will enable more subscribers to the platform to learn top-notch skills. Courses such as Musical instruments and Graphics designs shouldn’t be neglected, as people in this field of study will always want to improve their skills, Udemy providing series of quality courses for these subject, will not only increase subscribers  but the profit in time.






