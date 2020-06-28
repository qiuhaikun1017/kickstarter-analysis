# kickstarter-analysis
Performing data analysis to uncover trends
## Overview of Project
### Purpose

A fund-raising campaign is initiated by a play-writer, Louise, for her upcoming theatre play, _Fever_, and she is keen to discover what are the key factors to drive the successful outcome of a fundraising campaign. In this report, a data analysis is carried out in order to help her to uncover whether or not the likelihood of a “successful” outcome of fundraising campaign for a theatre play is associated with its launch date and fundraising goal amount. 


## Analysis and Challenges

To help Louise, a research is conducted based on a dataset of a sample of 4114 campaign projects. The dataset consists of valuable information of past campaign projects, which includes their: fundraising goal amount, the actual pledged amount, the campaign’s launch date and its ended date, the projects’ category, the country and the campaign’s outcome ( “successful”, “failed”, “live” or “cancelled”). We used Excel as the tool for examining this task and visualizing our result so the data can be more easily understood by a non-data analysis background individuals like Louise. 

### Part 1: Analysis of Outcomes Based on Launch Date

In the first part of our analysis, we focused on examining the change of number of outcomes based on the launch date, specifically we are looking at each month how the outcomes fluctuate. We begin our analysis by first reforming the data of launch date into regular “Year-Month-Day” form as the raw data included in the initial data sheet are in a form of “unix timestamp”, a form of expressing time into the number of second that have been spent since Jan 1st, 1970. We created a column called “Date created” by using the below codes:
>```=(((unix number/60)/60/24)+DATE(1970,1,1))``` 

to covert the unix form into date form and then formatted in date form. And then we created a new column called “Year” to extract the year of the “Date Created” column so that we are able to identify the range of year and later on use it as a filter when we organize the date. 

After the data is clean and ready to be analyzed, we use pivotable as the tool to conduct our research. The number of outcomes and its corresponding date are inputted into pivotable and “Year” and “Category” are used as filter. The below line chat shows that the fluctuation of outcomes for theatre campaign based on month from 2009 to 2017. Please note that label of each month means the total outcome of each month over the duration. For example, the number shown under “Jan”, means the total number of outcome for all the “Jan” from 2009 to 2017. 



According to the chart, the number of successful outcome hits the peak at May, which arrived 111. The least number of successful number happens in Dec, which is still higher than the number of failed and canceled at Dec. Furthermore, the overall count of successful outcome is higher than the overall count of failed and canceled respectively at each month.

#### Chanllenge for Part 1
However this graph does not tell us how specifically in each year the tendency of successful outcome has changed. For example, in certain year like 2009, there is no theatre shows has been fundraised, while from 2011 to 2013 all theatre campaign is successful. But in year 2020, is the data from 10 years ago still relevant to us? How the tendency in recent year tells us the story? To answer this question, We added the value of “Year” in the axis (Category), and we placed its order before “Date Created” so the graph shows the X-axis as the month of each valid year as below. 

It is clearly from the above chart that the number of successful outcome steadily remains below 5 per year from 2010 to 2013. Then in May of 2014, the total project of theatre shows dramatically climbed to 71, with 38 of them are successful. Followed by 2015, the magic May continues its legendary and achieved the highest number of successful campaign in that year. However, in both year 2015 and 2016, it is noticed that short after May, in June, the number of successful dropped dramatically and in March 2015 and Oct 2015 the failed counts outnumbers the successful number. **Overall, the Toal number of campaign and the number of successful campaigns shows a tendency of decreasing since 2016, _while the successful number remains higher than the failed ones at each month_**. 
 
 
### Analysis of Outcomes Based on Goals

### Challenges and Difficulties Encountered

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

- What can you conclude about the Outcomes based on Goals?

- What are some limitations of this dataset?

- What are some other possible tables and/or graphs that we could create?
