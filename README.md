# Project3
Team member: Yiling Du
The goal for this project is to use Python to analyze a big log file and generate some reports based on the data in the log file. Userlog.log file contains 5000 pieces of messages about 50 users’ login/logout activity and the 5000 messages are disordered, and each row has the date, time, activity, server, and user email id components. The reports that will be generated are suspicious, irresponsible, glitch, and domain.
##Suspicious activities: 
Suspicious activities mean if a user logs into any of the systems more than 5 times in a day, or if a user logs into any of the systems even once between 12:00 am to 5:00 am. In the suspicious_report, it will show the total amount of suspicious activities for 50 users, the total amount of suspicious activities for individual, and list individual’s email id, suspicious activities’ date, time, login/logout, server information on the specific suspicious day in ascending order based on the date and time.
##Irresponsible behavior: 
Irresponsible behavior means a user’s login amount is more than the logout amount in a day. In the irresponsible_report, it will show the total amount of irresponsible behavior for 50 users, the total amount of irresponsible behavior for the individual, and list individual’s email id, suspicious activities’ date, time, login/logout, server information on the specific irresponsible day in ascending order based on the date and time.
##System glitch: 
System glitch means a user’s login amount is less than the logout amount in a day. In the glitch_report, it will show the total amount of glitch for 50 users, the total amount of glitch for individual, and list individual’s email id, suspicious activities’ date, time, login/logout, server information on the specific glitch day in ascending order based on the date and time.
##Domain count: 
Domain name is the part after @ in the user’s email id. In the domain_report, it will show each domain name and the number of users is using that domain name, and how many different domain names the log file contains.

