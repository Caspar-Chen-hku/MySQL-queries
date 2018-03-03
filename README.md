# MySQL-queries
some practices in MySQL queries

## E-R Modeling
The **HKUber company** is designing a system to facilitate car sharing economy.  
The system hosts the following data:  

• The system stores *Member* information

• There are two types of membership: *Driver* and *Passenger*. A member can be both Driver and Passenger. 
1. For driver member, the system stores the *driving licence* and his/her *Bank account(s)*, which stores the unique accountID, owner name and issued bank. 
2. For passenger member, the system requires each passenger to register at least one *Credit Card* information

• A driver can register a number of *Vehicles* to the system

• The system stores *Trip* information.

▪ A passenger pays for the trip with one of his/her registered credit cards. The driver gets paid to one of his/her bank accounts. 

## Queries

1. Q0: Display *memberID*, *name* for all members. 

2. Q1: Display the *name* and *creditCardNO* of passengers with creditCardNO starting with 4384

3. Q2: Display the *memberID*, *passenger name* of the passengers who have not taken any trip

4. Q3: Display the *memberID*, *name* of user(s) who is both a driver and a passenger. 

5. Q4: Display the *locations* (source/destination) where driver with memberID = 3 has either picked up passengers from or dropped off passengers at. Combine the sources and destinations in one row with column name *“location”*. Each location should appear only once. List the locations in alphabetical order. 

6. Q5: For each driver, display the *memberID*, *name*, *licence* and the total value of *fare* earned. 

7. Q6: For each passenger that has taken more than one trip, display the *tripID*, *passengerID*, *source*, *destination*, *fare* of the trips, excluding the trip that the passenger paid the lowest amount of fare. Order the result first by descending order of passengerID, then by descending order of tripID if the passengerIDs are equal. 

8. Q7: For each referrer, show
• Referrer’s *memberID* (referrer) 
• *memberID*, *name* and the total *fare* of the referee who has spent the most amount in terms of total fare. 
• Order the result by ascending order of referrer 
• For referrer whose referees have not taken any trip, you may display the total fare = 0 (and display any of his/her referee) or ignore such referrer (omit that row). 

9. Q8
• Q8a: Display the drop-down menu showing the names of drivers. Add a submit button. After you click the submit button, the page will be redirected to q8b.php 
• Q8b: Display the passenger name, startDate and startTime of the trip that the selected driver from q8a has served. Make the name of the passenger as a hyperlink to q8c.php?driver=x&passenger=y (x is the memberID of the driver and y is the memberID of the passenger) 
• Q8c: Display the passenger name, startDate, startTime, source, destination, fare of the trips that the driver selected in q8a served passenger selected in q8b. 
