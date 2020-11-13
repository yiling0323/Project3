# Project3
Team member: Yiling Du 

The goal for this project is to use Python to analyze a big log file and generate some reports based on the data in the log file. Userlog.log file contains 5000 pieces of messages about 50 users’ login/logout activity and the 5000 messages are disordered, and each row has the date, time, activity, server, and user email id components. The reports that will be generated are suspicious, irresponsible, glitch, and domain. And eight additional analysis reports: dailyactivitycount, dailyservertcount, dailyserverleastpopular, dailyservermostpopular, datecount, serverdistribution, useractivitycount, usernamestartletter. (I uploaded the flowcharts for these additional analysis, see flowchartspartII for additional analysis)
## Suspicious activities: 
Suspicious activities mean if a user logs into any of the systems more than 5 times in a day, or if a user logs into any of the systems even once between 12:00 am to 5:00 am. In the suspicious_report, it will show the total amount of suspicious activities for 50 users, the total amount of suspicious activities for individual, and list individual’s email id, suspicious activities’ date, time, login/logout, server information on the specific suspicious day in ascending order based on the date and time.
## Irresponsible behavior: 
Irresponsible behavior means a user’s login amount is more than the logout amount in a day. In the irresponsible_report, it will show the total amount of irresponsible behavior for 50 users, the total amount of irresponsible behavior for the individual, and list individual’s email id, suspicious activities’ date, time, login/logout, server information on the specific irresponsible day in ascending order based on the date and time.
## System glitch: 
System glitch means a user’s login amount is less than the logout amount in a day. In the glitch_report, it will show the total amount of glitch for 50 users, the total amount of glitch for individual, and list individual’s email id, suspicious activities’ date, time, login/logout, server information on the specific glitch day in ascending order based on the date and time.
## Domain count: 
Domain name is the part after @ in the user’s email id. In the domain_report, it will show each domain name and the number of users is using that domain name, and how many different domain names the log file contains.
## Dailyactivitycount: 
This report shows each date’s the total number of login times and the total number of logout times. The date is in ascending order.
## Dailyservertcount: 
This report shows each date’s the total number of using each server’s times. The date is in ascending order.
## Dailyserverleastpopular: 
This report shows each date’s the most popular server(which server be used most for 50 users in a day). The date is in ascending order.
## Dailyservermostpopular: 
This report shows each date’s the least popular server(which server be used least for 50 users in a day). The date is in ascending order.
## Datecount: 
This report shows the number of activity times on the specific date of the 5000 pieces of activity information. The date is in ascending order.
## Serverdistribution: 
The report shows in the 5000 pieces of activity information, the total number of each server be used.
## Useractivitycount: 
The report shows the total number of each users’ login and logout times in the month. 
## Usernamestartletter: 
arrange the 50 users’ names depends on the first letter of their name. The report shows the users have the same first letter and show their whole email id. 
## 3 different errors:
1. I felt create and set a nested(two layer) dictionary is difficult, then I did some search and figured out I can do “dict1=dict.fromkeys(user_list,dict.fromkeys(date_list_sort))”, then add time, activity, and server information to the dict1[i][j].
2. I felt set a dictionary for the domain name is a little bit hard, then I looked up my notes for dictionary lecture, got more familiar with counting with dictionaries and using the knowledge .split(“@”) which learned in string lecture. 
3. Replicate some reports the same as the sample reports format is difficult. I tried my best to make my reports close similar to the example report. I used for loop, if condition, and update the string and cases count when the situation satisfices the condition


