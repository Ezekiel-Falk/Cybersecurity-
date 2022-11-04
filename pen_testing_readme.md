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


![SQL_Inject(2)](https://user-images.githubusercontent.com/88115439/200071305-d844c528-21ab-4931-bf84-67780611e21e.gif)
![SQL_Inject(0)](https://user-images.githubusercontent.com/88115439/200071306-da1770c4-e2c1-4d78-a265-306314df1bd2.gif)

## Red

Vulnerability #1: Brut Force with (Burp Suite Community)

Description: I Brut Forced the the Url id to find a hidden pages. By using a proxy connected to my browser I was able to try multiple numbers on the ID until I came across two hidden messages. 

![red4_burp_2](https://user-images.githubusercontent.com/88115439/200071334-9d099764-7a68-4902-beed-3f0d150ce0e0.gif)
![red3](https://user-images.githubusercontent.com/88115439/200071339-fca92da7-972f-4287-8c1e-f764a6c6d270.gif)
![red4_Burp](https://user-images.githubusercontent.com/88115439/200071342-348977ad-ce6e-4aeb-abfa-842522968d5d.gif)



## Green

Vulnerability #1: Cross site scripting (xss)

Description: For this  attack I started off with cross side scripting in the comments. With much success I was able to leave an alert.

![green(5_1)](https://user-images.githubusercontent.com/88115439/200071370-84ebd72f-0f6b-4a10-a47d-0ffb9803f283.gif)
![green(5)](https://user-images.githubusercontent.com/88115439/200071373-3c68f5bf-e1b3-45e1-b4ba-385288b236e9.gif)




## Notes

Describe any challenges encountered while doing the work

The only Callenges I encountered were trying to figure out what would be the best method of testing the web server for vulnerability.

