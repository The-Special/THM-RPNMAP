## THM-RPNMAP
 
**This article is a step by step walk-through of "RP: NMAP" and I would definitely say that if you haven't solved this challenge by yourself, please try harder and if you are still unable to figure things out. This walk-through is going to be your manual for this challenge.**
 
 
The main purpose of this room is to introduce nmap and teach us how to use them.
![Startup](https://i.hizliresim.com/DtBBQF.png)


## NMAP QUIZ


**Task 1**

You can find all the answers in this section from the help menu.

1-) First, how do you access the help menu?

-Answer : -h

*Usually shortcuts are the first letter of the word.*

2-) Often referred to as a stealth scan, what is the first switch listed for a 'Syn Scan'?

-Answer : -sS

3-) Not quite as useful but how about a 'UDP Scan'?

-Answer : -sU
*if you checking the "Help Menu" under the "Scan Techniques" you can find answers.*

4-) What about operating system detection?

-Answer : -O

*You can find in OS DETECTION menu.

5-) How about service version detection? 

-Answer : -sV

*You can find is SERVICE/VERSION DETECTION menu.*

6-) Most people like to see some output to know that their scan is actually doing things, what is the verbosity flag?

-Answer : -v

7-) What about 'very verbose'? (A personal favorite)

-Answer : -vv

8-) Sometimes saving output in a common document format can be really handy for reporting, how do we save output in xml format?

-Answer : -oX

*You can find in OUTPUT*

9-) Aggressive scans can be nice when other scans just aren't getting the output that you want and you really don't care how 'loud' you are, what is the switch for enabling this?  

-Answer : -A

10-) How do I set the timing to the max level, sometimes called 'Insane'?

-Answer : -T5

*You can learn more kind of timing in TIMING AND PERFORMANCE.*

11-)What about if I want to scan a specific port?

-Answer : -p

12-) How about if I want to scan every port?

-Answer : -p-

13-) What if I want to enable using a script from the nmap scripting engine? For this, just include the first part of the switch without the specification of what script to run.

-Answer : --script

14-) What if I want to run all scripts out of the vulnerability category? 

-Answer : --script vuln

15-) What switch should I include if I don't want to ping the host?

-Answer: -Pn

## NMAP SCANING

**TASK 2**

1-) Let's go ahead and start with the basics and perform a syn scan on the box provided. What will this command be without the host IP address?

*Just look Task 1*
-Answer : nmap -sS

2-) After scanning this, how many ports do we find open under 1000?

Solution :
          ![2](https://i.hizliresim.com/gbbRqm.png)

-Answer : 2

3-) What communication protocol is given for these ports following the port number?

Solution :![3](https://i.hizliresim.com/FkC33Q.jpg)

-Answer : tcp

4-) Perform a service version detection scan, what is the version of the software running on port 22?

Solution :![4](https://i.hizliresim.com/AAYWF5.png)

-Answer : 6.6.1p1

5-) Perform an aggressive scan, what flag isn't set under the results for port 80? 

Solution :
          ![5](https://i.hizliresim.com/QVnBr5.png)

-Answer : httponly

6-) Perform a script scan of vulnerabilities associated with this box, what denial of service (DOS) attack is this box susceptible to? Answer with the name for the vulnerability that is given as the section title in the scan output. A vuln scan can take a while to complete. In case you get stuck, the answer for this question has been provided in the hint, however, it's good to still run this scan and get used to using it as it can be invaluable. 

Solution :
          ![6](https://i.hizliresim.com/y0O3c8.png)

-Answer : http-slowloris-check

*If you look carefully can find Dos attack name.*



