# Pen Testing Live Targets

Time spent: **10** hours spent in total

> Objective: Identify vulnerabilities in three different versions of the Globitek website: blue, green, and red.

The six possible exploits are:

* Username Enumeration
* Insecure Direct Object Reference (IDOR)
* SQL Injection (SQLi)
* Cross-Site Scripting (XSS)
* Cross-Site Request Forgery (CSRF)
* Session Hijacking/Fixation

## Blue

Vulnerability #1: SQL Injection (SQLi) 

Description: I tested SQL Injection in the url by changing the id of one of the salesperson. After this I then tested to see if I had access to the database (Database Query Failed) which I did. Lastly I went ahead and put the database to sleep for 10 seconds secwith a SQL Injection ' OR SLEEP(15)=0--'

![Alt text](SQP_Injection(0).gif) 
![Alt text](ezgif.com-gif-maker(1).gif)

## Red

Vulnerability #1: Brut Force with (Burp Suite Community)

Description: I Brut Forced the the Url id to find a hidden pages. By using a proxy connected to my browser I was able to try multiple numbers on the ID until I came across two hidden messages. 
![Alt text](red3.gif)
![Alt text](red4_Burp.gif)
![Alt text](red4_burp_2.gif)



## Green

Vulnerability #1: Cross site scripting (xss)

Description: For this  attack I started off with cross side scripting in the comments. With much success I was able to leave an alert.

![Alt text](green(5).gif)
![Alt text](green(5_1).gif)

## Notes

Describe any challenges encountered while doing the work

The only Callenges I encountered were trying to figure out what would be the best method of testing the web server for vulnerability.

