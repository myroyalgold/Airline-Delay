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
This data was imported as a csv file on Excel.
To do this, I click on get data, then select text/csv 

![2022-07-16](https://user-images.githubusercontent.com/107118603/179371695-2dd042da-b670-45db-8eb6-d203569cc836.png)


after that, I locate where the csv file is on my system
![2022-07-16 (1)](https://user-images.githubusercontent.com/107118603/179372393-83aeb77e-5a1e-4ddd-979e-0f0086429029.png)

I click on transform data to clean the data
![2022-07-16 (2)](https://user-images.githubusercontent.com/107118603/179372447-bf75963e-eab8-4918-b246-83393848f37b.png)


the table was cleaned to remove all duplicate and error values.
![2022-07-16 (3)](https://user-images.githubusercontent.com/107118603/179372481-bdae3409-6ce1-484c-a982-80bb87eac73d.png)


I impoterd delayed data set from kaggle to predict causes of airline delay, alighted the columns needed and unpivot others.
![2022-07-16 (10)](https://user-images.githubusercontent.com/107118603/179372556-ef1e70f2-b24b-455f-9310-cb8e9a2491a1.png


i removed all the duplicate and error values in the dataset.
To do this;
click on transform,click on drop down beside remove rows, this will enable you to remove blank, null, duplicate and error values.
![2022-07-16 (13)](https://user-images.githubusercontent.com/107118603/179372681-a24606fb-9c6b-4ee3-9b18-47abaeb84e2d.png)

After doing this, i realised there are null values in the data, then i proceed to replace all the null values to 0.
I click on Transform in the query pane, Select Replace value, and it prompts a dialogue box asking for value to find and what to replace it with.
![2022-07-16 (14)](https://user-images.githubusercontent.com/107118603/179372820-d69e3f33-0263-4506-95d5-b35f0ad5b8a5.png)
![2022-07-16 (15)](https://user-images.githubusercontent.com/107118603/179372895-a2b5b993-0cba-4f1d-828c-6beb0a0e853d.png)


When i click on close and apply, the delayed dataset rows is much and it display some errors, i rightclick on the delayed dataset, edit and it direct me to query page.
![2022-07-16 (16)](https://user-images.githubusercontent.com/107118603/179372919-17636d3c-574f-4c83-8b87-e181873b3390.png)

I click on Home, keep rows and input the rows i want.
![2022-07-16 (17)](https://user-images.githubusercontent.com/107118603/179372986-bb12685e-eae1-4e90-b0fe-b4893cce06eb.png)

Yes!!!
The dataset is reduced to exact rows as in Airline and the file was saved as an Excel file.
![2022-07-16 (18)](https://user-images.githubusercontent.com/107118603/179373038-6bd28f71-dbd9-4e9c-8b4b-3412684a5f48.png)


####It's time for Microsoft PowerBi
![2022-07-16 (19)](https://user-images.githubusercontent.com/107118603/179373077-761cab89-dbc3-4d15-ad54-a2e0d672119a.png)

Dont forget i save my data as excel file on my sytem, its time to bring it in here.
To get data from Excel file i followed the following steps;
Home, getdata and select Excelworkbook.
![2022-07-16 (20)](https://user-images.githubusercontent.com/107118603/179373147-cfc9bba0-7b79-487e-b4e7-490ef28f6aad.png)

locate where the file is
![2022-07-16 (21)](https://user-images.githubusercontent.com/107118603/179373155-35049da8-c8b4-46dd-b656-78aec844e440.png)


Note: while i was opening my data on excel i click on transform data to clean my dataset but here i select load because the data was already cleaned and formated.

I had to choose the table i want to work with and I chose both  Airline and delayed flights tables...
![2022-07-16 (22)](https://user-images.githubusercontent.com/107118603/179373186-4f608b64-1347-4db5-b101-64de1dc62379.png)

My dataset is loading...
![2022-07-16 (23)](https://user-images.githubusercontent.com/107118603/179373224-0778d578-4cf8-4f1a-971c-ad745e4154f1.png)

I design the dashboard format in my notebook then later design the layout here
![2022-07-16 (26)](https://user-images.githubusercontent.com/107118603/179373352-331479cb-f04a-4317-b17a-0d134cf4c884.png)


also, some calculated measures were obtained such as;
•	Delay flights: (Where delay value equals 1) which was obtained by filtering and counting all the values of 1[ i.e. True ] in Delay columns.
![2022-07-16 (27)](https://user-images.githubusercontent.com/107118603/179373340-b9991692-5684-49c0-9e9d-5ac1b887517b.png)



•	Flight on time: This was obtained by filtering and counting all the values of 0 in delay columns.
![2022-07-16 (28)](https://user-images.githubusercontent.com/107118603/179373364-0316fe98-7805-4b1e-8ebf-43e81ad0ce06.png)


•	Total flights :( Delay flights) + (flights on time)
![2022-07-16 (30)](https://user-images.githubusercontent.com/107118603/179373381-789971ac-262b-42a0-9194-dcc552f60c9e.png)



•	Delay Index: This is the percentage of delay and it was calculated by ( Delay flights /Total flights) * 100
![2022-07-16 (31)](https://user-images.githubusercontent.com/107118603/179373389-47469afa-33d0-46a2-a84f-de37975474dd.png)

•	Delayed dataset that was imported and cleaned have six attributes which are the causes of delay flights. The attributes are; carrier delay, weather delay, NAS delay, late aircraft delay, arrival delay and departure delay.


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
