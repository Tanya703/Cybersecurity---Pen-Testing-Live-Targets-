
# Pen Testing Live Targets

Time spent: 3 hours spent in total

> Objective: Identify vulnerabilities in three different versions of the Globitek website: blue, green, and red.

The six possible exploits are:

* Username Enumeration
* Insecure Direct Object Reference (IDOR)
* SQL Injection (SQLi)
* Cross-Site Scripting (XSS)
* Cross-Site Request Forgery (CSRF)
* Session Hijacking/Fixation

Each color is vulnerable to only 2 of the 6 possible exploits. First discover which color has the specific vulnerability, then write a short description of how to exploit it, and finally demonstrate it using screenshots compiled into a GIF.

## Blue

Vulnerability #1: SQL Injection (SQLi)

Description: Used single qoute to test if SQL injection can be performed. After getting "Database query failed" message, used ' OR SLEEP(10)=0--' statement in URL for id to put the database to sleep for 10 seconds.

<img src="Blue Taget 1 SQL Injection.gif" width="800">


## Green

Vulnerability #1: Cross-Site Scripting (XSS)

Description: In the feedback form I put <script>alert('Tanya found the XSS!');</script>. When logged in to check feedback the alert poped up.

5. Cross-Site Request Forgery: One of the three s

<img src="Green Taget 1 Cross-Site Scripting.gif" width="800">


## Red

Vulnerability #1: Insecure Direct Object Reference (IDOR)

Description: I found an unfilled space under MA state under find a saleperson tab. Opened a page of the salesperson above. Checked his id number in URL. Submitted a new URL with id incremented by 1 and got access to hidden user's page.

<img src="Red Taget 1 IDOR.gif" width="800">


## Notes

Describe any challenges encountered while doing the work
