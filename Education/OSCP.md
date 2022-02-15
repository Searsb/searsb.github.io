---
title: OSCP Experience
---

I passed the Offensive Security Certified Professional (OSCP) exam in December 2021 on my third attempt. I really enjoyed and respect the whole entire process of becoming OSCP certified.

<div data-iframe-width="150" data-iframe-height="270" data-share-badge-id="e87bf65e-918b-4658-b7f6-f9a39538dadc" data-share-badge-host="https://www.credly.com"></div><script type="text/javascript" async src="//cdn.credly.com/assets/utilities/embed.js"></script>


* 
{:toc}

## Introduction and Prep for the OSCP

In August of 2020 I began "Applications of Cybersecurity" at Trine University. The professor used the PWK material as our textbook and for assignments. I had never heard of the OSCP before looking into this class. I was familiar with Kali Linux and some other basic tools from my home lab back in high school but I was without direction and ignorant of all of the resources that were out there to help a student like myself learn. 

Trine purchased the PWK 60 Days and an exam attempt plus a 30 day lab extension. Doing the PWK in the classroom was advantageous at the time for me because I lacked the discipline to focus and do the lab exercises by myself. At the end of the semester I actually forgot to do and turn in the very last exercises from the book due to focusing on other finals. The final in that class was to do a vulnerability scan and evaluate different ways to attack our targets in the lab environment. We were not required to pwn any machines in the lab environment. I did end up compromising an AD environment (by accident it seems like looking back now) after this I was hooked on hacking though! My number of lab boxes compromised probably plays with the OffSec's numbers on how many boxes are on average pwned to pass the OSCP.  

The next semester was under the same professor and instead of studying for the OSCP we were studying for the CISSP certification. Our homework in that class was to  work through Hack The Box Machines. We had to pwn up tp two retired boxes a week and for the midterm and final we were assigned university dedicated boxes. There were no write ups available and no dedicated forums for those boxes to look up answers, next steps, or hints. At the end of this semester, my OSCP Exam attempt was about to expire so I set a date and time and prepared for this exam!

## Attempt 1 - Fail

Date: April 10th 2021
Time: 22:00 EST

My first attempt was disastrous. By the time I scheduled the exam the only available start time was 23:00. For most college students this wouldn't be a problem but I am a morning person not an evening person, typically I'm in bed by 21:00.  I was also the first person I know to have taken the test personally and no amount of reading online truly prepared me for it. I took the test in my office. I bought snacks( more on my snack choice later.), soda, even a small camping mattress and a small pillow with a blanket to take naps and breaks.

I managed to get the buffer overflow box(BOF). I honestly love BOF. In my opinion BOF is the most pure form of hacking. It doesn't allow you to take someone else's exploit and re-use it. I love diving into the register and handling hex code. I plan on taking the EXP-301 and EXP-401 in the future as well to fill this desire for knowledge.

I also managed to get the ten point box but that was it for my first attempt. I just followed way too many rabbit holes and worked myself in circles. But I wasn't too discouraged. I knew my major points of failure.  I worked on the following goals:

* Schedule a better time for the test that worked with my normal sleep schedule
* More practice
* Set a limit on how long I spend on each possible vector of attack

## Attempt 2 - Fail
Date: July 31st 2021
Time: 08:00 EST

I purchased the 2nd attempt and scheduled it for late July. At this point I was now working at the university full time. I had graduated in the spring and the university liked my work so much that I was offered a full-time position doing the same work I had been doing as an intern. I am also a high school football official and football season began in august; I needed to take the test before I began officiating football.

To prepare for the second test I scheduled a better time. As soon as I purchased the test, I looked at my calendar and scheduled the test for a Saturday morning at 8am. 

I had also purchased a Hack The Box Subscription(HTB) subscription. My goal was to do a box a week if not more. At the time of the test I had completed all of the active easy and medium boxes. I intended to get write ups of the HTB boxes as they are retired in the future on this site as well.

When this exam began I was more prepared and confident! I had created a schedule for when and how long I planned to spend on each box initially. At the time I was also ordering from the meal delivery service, "Hello Fresh" so the day before the exam I cooked up several meals and stored them in the fridge.  Again, I brought snacks and some caffeinated drinks.

This time I did not bring a mattress with me to my office to relax. I had realized it was too easy to relax and get lost in my phone instead of letting my mind truly relax. 

At 07:30 I began logging in and prepared to connect to the exam session. At 7:45am I logged into the exam session and started the verification process. At 8am I began the test. I managed to get the BOF(25pts) easily again. I have a set of python files that goes through the basic steps of the buffer that requires only minor modification. I also managed to get the 10pt(35pts) box again. I then spent a lot of time on a 20 point box and managed to get the initial shell but no priv esc (45pts). Next, much time was spent searching and enumerating the 25pt box. I was not able to get anything for a while and by this time I was hungry for dinner and took a break. 

I went on a small mile bike ride, took a shower, and ate dinner. I think the bike ride and getting the blood pumping really helped me mentally. I managed to get a foothold on the 25 pointer box (57.5pts). I then worked on the priv esc which was pretty straightforward and fully pwnd the box(70pts)! I had the points needed to pass but still had time left so I focused on the last 20 point box. Sadly I was not able to get it. I had tunnel vision on what I believed to be the exploitable services and was not able to enumerate any further. I ended my exam about an hour early after running through all of the boxes again and confirming that I had all the required documentation. 

I turned in my report.  Three days later I was informed that I had failed.  Initially it did not say why I failed but being so close I knew it could be anything. My report was reviewed upon request and I was informed that I had missed documenting a crucial step in my report. It was in my notes but not in the final report! I understand completely why I failed. Documentation is important and I had made a crucial mistake. However, I was greatly encouraged, more than ever I was ready to take the test again as soon as the cool down period ended!  I learned the following lessons after this second attempt:

* Take the time to read and re-read the report to confirm everything is there.
* Create a list of possible attack vectors and cross them out as they are ruled out.

## Attempt 3 - Pass

Original Date: January 22nd
Original Time: 09:00 EST

Date: December 4th
Time: 04:00 EST

The third and final exam attempt was a long time coming. OffSec was in the middle of migrating to their new platform and my account got caught somewhere in the middle. My account had several issues that may have caused problems with migration which I won't get into. After a lot of back and forth I finally gained access to the exam ordering link and then after some more back and forth I gained access to the scheduling link. After reviewing the available times I decided to take the test at 09:00 on January 22nd. The weekend before I received the paper certificate actually!

As most of the readers of this article know, OffSec updated the exam January 11th but notified the public late November. I had recently started a new job as a Jr Security Analyst when this news was released. I decided to move my test up so I could take the older version of the test I was familiar with. There were a few issues with this though. The first one being scheduling so late left me with very limited options. The only date that worked was that weekend at 4am. My new employer's Christmas party was the day before and I had already RSVP'd. So I made the decision to go to the Christmas party, eat the wonderful food and as soon as I ate dinner I ran home to get as much sleep as I possibly could.

Again, I prepared lunch and dinner a few days before as well as buying several snacks. For this test I decided to make a paper checklist for every box with the basic enumeration steps Available Services, Foothold, Priv Esc, Etc. I used this checklist when writing the report to confirm I had every step in the report. I was not going to fail the same way twice. I don't remember where I heard it but writing the report as you go is helpful. With all of these checks in place I was prepared.

On this third attempt I got very lucky. The 25 point box was actually the box I messed up on in my report on attempt number 2. This was my chance to redeem myself! Immediately I knew that I had 50 points(BOF + 25)! Unfortunately, one of the 20 pointers was the box I was not able to even get a foothold on attempt number two. I managed to get the 10 pointer very easily(60 pts). I worked on the "new" 20 pointer for a while and made no progress. After eating a late lunch I decided to work on the "old" 20 pointer I got stuck on in the 2nd attempt. Right before dinner I found my foothold(70pts)! I had to keep reminding myself to not get stuck in rabbit holes. I found myself going down the same paths I tried in the first attempt even though they didn't work. Taking deep breaths and breaks is essential! After getting the foothold I had the points to pass! I wrote down what I needed to remember and took a break for dinner. I had a full 20 pointer and half of the 20 pointer left. After dinner I worked on the report for a few hours and compromised all the boxes again from the starting configuration confirming the report had all of the steps needed.

After I confirmed the report was good I went to work on the last three flags. Again I was not able to find any of them. So at 03:30 I called it a day. I let the proctors know to shut down my lab environment and went to bed. Sunday I cleaned up my report and made it more professional looking. I then followed the exam guide on how to upload the report and turned it in Sunday evening.  

Waiting for exam results like this is agonizing especially when you are on the brink of passing or failing. Tuesday after I turned in the test I was driving to work and got an email from OffSec. On my phone it gives me a preview of what is in the body of the email and all I read was "We are happy to inform you..." and I knew I passed! At this time I was driving so I couldn't read the full email and had about another 20 minutes before I could.  Those 20 minutes were especially difficult as I was concerned that I may have misread the email heading.  I am happy to say that I did indeed pass!

## Recap & Tips

The OSCP is a great test! I have always been a good traditional test taker so the hands on aspect of this test was a welcomed challenge and change of pace. I am not against the changes OffSec made to the OSCP. I think they are great changes especially since starting my new job securing an enterprise AD environment. I personally was just not ready or prepared for the new exam format and I was regretting not scheduling the test earlier in the first place. 

In regards to the proctoring software and proctors I had no issues. They were all pleasant to work with. The closest thing to an issue I had was needing to restart my host machine and then reconnect to the proctor software. I took lots of water breaks. I have a large 32oz cup that I refilled at least twice an hour. All the proctors asked was to let them know when you left and returned.

I mentioned all the snacks I had purchased and after the third exam I realized the mistakes I made in my snack choice. I chose things like M&Ms and Twizzlers. Besides water I drank Dr. Pepper or Cherry Pepsi. The high caffeine and sugar intake upset my stomach and muddled my energy levels. I suggest no more than a cup of tea to start the day and soda pop only in the late evening to get through the night if needed. Healthy snacks are a must as well!

During the exam I suggest the following:

* Tried and true note taking system that you know
	* I used Cherrytree and Word for my notes (Currently migrating to Obsidian)
* A timer to force yourself to change direction if you are stuck in a rabbit hole
	* No more than thirty minutes per attack vector
* Physically visualize machines you are stuck on
	* Draw/list attack paths
	* Cross out things you tried that didn't work so you don't repeat yourself
* Remember the test is designed to be taken in under 24hrs!!
* Lots of water breaks
	
## Certification

The initial email stating that I had passed contained the links to claim the certification on Credly. The email contained the link to send OffSec the delivery information. I filled this out the day of (Jan 7th). I received the paper certtificate about 50 days later. There are several reasons why it took so long; it was the holiday season, employees on vacation and shipping disruptions. 

### Dates Recap
* Exam 1 - April 10th, 2021
* Exam 2 - July 31st, 2021
* Exam 3 - December 4th, 2021
* Results - December 7th, 2021
* Shipping Information Sent - December 7th, 2021
* Original Exam 3 - January 22, 2022
* Tracking Information Received - January 26th, 2022 
* Packaged Received - January 26th, 2022

## Future

I am currently studying for PEN-300/OSEP. I purchased the learn ONE subscription in late December while it was discounted. I have already learned much and I am looking forward to the 48hr exam. My long term goals is to go for the trifecta OSEP. OSED, and OSWE (OSCE3). I am also looking into working on developing boxes for OffSec and HTB. But my next major project is helping to design the [Bsides Fort Wayne](https://bsidesfortwayne.org/) CTF!