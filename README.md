# Hotel_Booking_Data_analysis
Analyzing the Data of Hotel Bookings
Objective
We are provided with a hotel bookings dataset.

Out main objective is perform EDA on the given dataset and draw useful conclusions about general trends in hotel bookings and how factors governing hotel bookings interact with each other



Dataset

We are given a hotel bookings dataset. This dataset contains booking information for a city hotel and a resort hotel. It contains the following features.

- hotel: Name of hotel ( City or Resort)
- is_canceled: Whether the booking is canceled or not (0 for no canceled and 1 for canceled)
- lead_time: time (in days) between booking transaction and actual arrival.
- arrival_date_year: Year of arrival
- arrival_date_month: month of arrival
- arrival_date_week_number: week number of arrival date.
- arrival_date_day_of_month: Day of month of arrival date
- stays_in_weekend_nights: No. of weekend nights spent in a hotel
- stays_in_week_nights: No. of weeknights spent in a hotel
- adults: No. of adults in single booking record.
- children: No. of children in single booking record.
- babies: No. of babies in single booking record. 
- meal: Type of meal chosen 
- country: Country of origin of customers (as mentioned by them)
- market_segment: What segment via booking was made and for what purpose.
- distribution_channel: Via which medium booking was made.
- is_repeated_guest: Whether the customer has made any booking before(0 for No and 1 for 
                     Yes)
- previous_cancellations: No. of previous canceled bookings.
- previous_bookings_not_canceled: No. of previous non-canceled bookings.
- reserved_room_type: Room type reserved by a customer.
- assigned_room_type: Room type assigned to the customer.
- booking_changes: No. of booking changes done by customers
- deposit_type: Type of deposit at the time of making a booking (No deposit/ Refundable/ No refund)
- agent: Id of agent for booking
- company: Id of the company making a booking
- days_in_waiting_list: No. of days on waiting list.
- customer_type: Type of customer(Transient, Group, etc.)
- adr: Average Daily rate.
- required_car_parking_spaces: No. of car parking asked in booking
- total_of_special_requests: total no. of special request.
- reservation_status: Whether a customer has checked out or canceled,or not showed 
- reservation_status_date: Date of making reservation status.



Data Cleaning

(1) Removing Duplicate rows
All duplicate rows were dropped.

(2) Handling null values
Null values in columns company and agent were replaced by 0.
Null values in column country were replaced by 'others'.
Null values in column children were replaced by the mean of the column.

(3) Converting columns to appropriate data types
Changed data type of children, company, agent to int type.
Changed data type of reservation_status_date to date type.

(4) Removing outliers
One outlier was found in the adr column. Simply dropped it.

(5) Creating new columns
Created new column total_stay by adding stays_in_weekend_nights+stays_in_week_nights.
Created new column total_people by adding adults+children+babies.


Exploratory Data Analysis

Q1) Which agent makes the most no. of bookings?

 Q2) Which meal type is the  most preffered meal of customers?

 Q3) What is the  percentage of bookings in each hotel?

 Q4) Which is the most common channel for booking hotels?

 Q5) Which are the most busy months?

 Q6) From which country most of the guests are comin ?

 Q7)  Which hotel seems to make more revenue?

 Q8)  Which hotel has a  higher lead time?

 Q9)  Which hotel has higher bookings cancellation rate.

 Q10)  Which channel is mostly used for the  early booking of hotels?

 Q11)  Which channel hasa  longer average waiting time?

 Q12)  Which distribution channel brings bettern revenue-generating deals for hotels?

 Q13)  Which significant distribution channel has the highest cancellation percentage?

 Q14) What is the trend of bookings within a month?

 Q15) Which types of customers mostly make bookings?



 Conclusion

1.	City hotels are the most preferred hotel type by the guests. We can say City hotel is the busiest hotel.

2.	27.5 % bookings were got cancelled out of all the bookings.

3.	Only 3.9 % people were revisited the hotels. Rest 96.1 % were new guests. Thus retention rate is low.

4.	The percentage of 0 changes made in the booking was more than 82 %.  Percentage of Single changes made was about 10%.

5.	BB( Bed & Breakfast) is the most preferred  type of meal by the guests. 

6.	Maximum number of guests were from Portugal, i.e. more than 25000 guests.

7.	Average ADR for city hotel is high as compared to resort hotels. These City hotels are generating more revenue than the resort hotels.

8.	Booking cancellation rate is high for City hotels which almost 30 %.

9.	Average lead time for resort hotel is high.

10.	Waiting time period for City hotel is high as compared to resort hotels. That means city hotels are much busier than Resort hotels.

11.	Resort hotels have the most repeated guests.

12.	In July and August had the most Bookings because of Summer vaccations.

13. 'Online T/A' has the highest cancellation in both type of Hotels

14. In order to reduce the booking cancellations, hotels need to set the refundable/no refundable and deposit policies..

And many more conclusions.
