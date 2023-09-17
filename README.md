# EDA-Capstone-Hotel-Analysis

Hotel Bookings Exploratory Data Analysis
Objective
We are provided with a hotel bookings dataset.
Out main objective is perform EDA on the given dataset to get the listings of hotel bookings and how factors governing hotel bookings interact with each other.
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
Data Cleaning and Feature Engineering
(1) Removing Duplicate rows
All duplicate rows were dropped.

(2) Handling null values
Null values in columns company and agent were replaced by 0.
Null values in column country were replaced by 'others'.
Null values in column children were replaced by the mean of the column.
 Creating new columns
Created new column total_stay by adding stays_in_weekend_nights+stays_in_week_nights.
Created new column total_people by adding adults+children+babies.
Mainly performed using Matplotlib and Seaborn library and the following graph and plots had been used:

Bar Plot.
Histogram.
Scatter Plot.
Pie Chart.
Line Plot.
Heatmap.
Box Plot

Conclusion of EDA Project
First of all we saw the hotel was booked the most in 2016
Percentage stay of adults per month 
Numerical distribution using heatmap
total stay of passengers per monthwise
It has been concluded that trasient type used City hotel the most for stay
PRT country has the highest no of bookings
Most demanded room type is A, but better adr rooms are of type H, G and C also. Hotels should increase the no. of room types A and H to maximise revenue
200000 customers are of no deposit type
Room category A has been mostly preferred by the customers of the Resort Hotel
The most used means of distribution channel by the customers is TA/TO
As per the reservation type most customers have checked out from the hotels means bookins were more as cvomparative to cancelled and No show
City hotel has been preferred the most for the stay by the customers
We can see that graph Arrival_num has small peaks at regular interval of days. This can be due to increase in arrival weekend.
