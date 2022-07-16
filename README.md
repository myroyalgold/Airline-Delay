# AIRLINE DELAY
A flight delay is when an airline flight takes off and/or lands later than its scheduled time.


### PROBLEM STATEMENT
The purpose of this data set is for predicting whether a given flight will be delayed, and telling a story about the entire flight experience.

### PROBLEM OBJECTIVES
What has been the history of flight experiences in the past?
How bad was delayed flights?
Any identified pattern with delayed flights?
Which Airline has the most delayed flight?
Which Airline is best to fly?
Which Airport has the highest frequency of delay?
What is the Average Length and Time Flight by Airlines?
What is the percentage of delay to flight on time?


### DATA SOURCING
This data is a capstone dataset given by OYINBOOKE After the completion of #30daysoflearning and  here is the link to the data. https://github.com/theoyinbooke/30Days-of-Learning-Data-Analysis-Using-Power-BI-for-Students/blob/main/Airline%20Project/Airlines.csv

### DATA TRANSFORMATION
This data was imported as a csv file on Excel
To do this, click on get data
![2022-07-16](https://user-images.githubusercontent.com/107118603/179371695-2dd042da-b670-45db-8eb6-d203569cc836.png)

the table was cleaned to remove all duplicate and null values and the day of the week was later derived by using a DAX function.
also, some calculated measures were obtained such as;
•	Delay flights: (Where delay value equals 1) which was obtained by filtering and counting all the values of 1[ i.e. True ] in Delay columns.
•	Flight on time: This was obtained by filtering and counting all the values of 0 in delay columns.
•	Total flights :( Delay flights) + (flights on time)
•	Delay Index: This is the percentage of delay and it was calculated by ( Delay flights /Total flights) * 100
•	Flight Index : This is the percentage of flight on time and it was calculated by ( Flights on time /Total flights)
•	Delayed dataset was also imported and cleaned to six attributes which are the causes of delay flights. The attributes are; carrier delay, weather delay, NAS delay, late aircraft delay, arrival delay and departure delay.


#### Yes!!! it's time to tell a story
This is the first page in which you can navigate to view any of the pages.
There are 4 buttons there,Delay report, Flight report, and Dashboard. when you click on any button it will direct you to a specific page as it was been set by the button action. 
![2022-07-16 (33)](https://user-images.githubusercontent.com/107118603/179371759-ddd115de-cd9c-4f34-80f9-02272acc2090.png)


#### This second image answer the following questions...
How bad was delayed flights per weekday?
What is the total delayed flights?
Which Airline has the most delayed flight?
Which Airline is best to fly?
What is the frequency of delay per year?
What is the frequency of flights per weekday?
![2022-07-16 (34)](https://user-images.githubusercontent.com/107118603/179371769-1fd48324-3ec7-4e80-9721-7aec3432c51d.png)


#### This page gives review to
Causes Of Airline Delay?
Airport with the highest frequency of delay.
The Average Length of flight by Airlines. 
The Average Time of flight by Airlines. 
The percentage of delay to flight on time.
![2022-07-16 (35)](https://user-images.githubusercontent.com/107118603/179371788-d481961b-3bdf-4850-947e-07d84acaf05d.png)


#### Dashboard 
This will help you track identified pattern with delayed flights as it display all the answers to the earlier stated questions.
![2022-07-16 (36)](https://user-images.githubusercontent.com/107118603/179371790-d8789bda-e8ad-4925-b8fb-85b677d59dec.png)

### DATA INSIGHTS
From this analysis, we can infer that;
•	There was a total of 539,383 Total flights by different 18 Airlines.
•	240,264 was recorded as the delayed flights.
•	299,119 was recorded as the flight on time.
•	In 1899 there was a total of 34,030 flight delay, while in 1900, total delayed flights of 206,234 was recorded.
•	The most delayed Airline is WN.
•	FL Airline spends more time, CO Airline is flights  for longer distance.
•	HA Airline is recommended as the best Airline to fly because it has the least number of flight delay.
•	DelayIndex/Percentage is 45% while that of flight on time is 55%.
NOTE: Source Airport is also known as Airport from and Desination Airport is Airport to.



#### FINDINGS
Full meaning of abbreviations used for Airlines and Airports.
![2022-07-16 (37)](https://user-images.githubusercontent.com/107118603/179372270-3cf84de2-e9cc-457c-91e6-7faa51b10d48.png)


### RECOMMENDATION 
•	I found out that People flights with the most delayed Airlines.
•	It is better to book an early flight to avoid arrival and departure delay.
•	Airlines can reduced delays by inflating the scheduled time of the flight
•	Schedule your flights for weekends to avoid delay.
•	Weather Analysis should be done before Airline moves.
