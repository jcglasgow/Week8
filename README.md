# Week8

# Project 8 - Pentesting Live Targets

Time spent: 10 hours spent in total

> Objective: Identify vulnerabilities in three different versions of the Globitek website: blue, green, and red.

The six possible exploits are:
* Username Enumeration
* Insecure Direct Object Reference (IDOR)
* SQL Injection (SQLi)
* Cross-Site Scripting (XSS)
* Cross-Site Request Forgery (CSRF)
* Session Hijacking/Fixation

Each version of the site has been given two of the six vulnerabilities. (In other words, all six of the exploits should be assignable to one of the sites.)

## Blue

Vulnerability #1: Session Hijacking

Open a hacktools from one session (green) and copy to the session ID of blue. If green were logged in, blue would also be logged in.
![](https://imgur.com/taylzeU)


Vulnerability #2: SQL injection

By inserting SLEEP script in the url, the command is shown to have been executed by waiting 5 seconds.

![](https://imgur.com/JdwpErw)

## Green

Vulnerability #1: User Enumeration

When attemping to login with an existent user in the database versus a non-existent user, the message returned has different formattting (bold vs non-bold).

![](https://imgur.com/jiX7ykF)

Vulnerability #2: XSS

The feedback parameter is vulnerable to XSS.
![](https://imgur.com/f5YS89W)

## Red

Vulnerability #1: IDOR

By changing the id in the PHP in the url, hidden data can be accessed.

![](https://imgur.com/Izd8loD)

Vulnerability #2: CSRF


## Notes

Describe any challenges encountered while doing the work
