---
layout: post
title: A new dimension
---

Last week was pretty uneventful.
---

Nothing big happened. Just the usual grind of assignments and work and stuff. This week's CS314 assignment took me forever to code and debug,and it really screwed up my schedule. I planned on getting started on Node.js on Friday and then Saturday was project day with Sohaib and Sunday was studying for the calc test on Monday, but that completely got thrown off due to my carelessness =(.

Why my schedule got screwed
---

We had to write an [Anagram Solver](http://www.cs.utexas.edu/~scottm/cs314/Assignments/A8_Anagrams.html) from scratch. I screwed up the efficiency of my subtract method within the LetterInventory class, and I ended up thinking that it was the main recursive call that was inefficient. Spend a good amount of time in office hours trying to work this through with my TA, but he didn't see any issue either. Wasn't until a good bud of mine, Jamin, suggested that I look into subtract. Ran some time tests on it, and turned out it was O(M^2) as opposed to O(M). FeelsBadMan

Well anyway, onto the more exciting stuff, me and Sohaib finished base functionality with Amazon Alexa! God bless the persion who wrote [this article](https://developer.amazon.com/public/community/post/Tx14R0IYYGH3SKT/Flask-Ask-A-New-Python-Framework-for-Rapid-Alexa-Skills-Kit-Development). Had she not written it, we would have had to resort to JS, which both of us have no clue how to do. But yeah, being able to utilize flask made things so much easier. Writing the framework took no time at all, and by 12:30, we had a working version (we started at 10). It worked EXCEPTIONALLY well. I was super surprised.

Sure does seem good and dandy right?... Well....
---
Well what? Well turns out Amazon Web Services screwed us again! They forced us to run our scripts on their lambda platform, and if you read my last post, Flask and AWS do not mix well. 4 hours were spent attempting to use Lambda, until I just told Sohaib to host it via [PythonAnywhere](https://www.pythonanywhere.com/) and just force device invoking our skill to send HTTP requests to the server to get the information. And then came a lot of errors. First wave of errors were fixed by importing our alexa flask-ask package via console (NOTE: DO NOT USE sudo pip install, it WONT WORK. Use [THIS](https://help.pythonanywhere.com/pages/InstallingNewModules/) instead.). Second wave of errors were because of the restrictions placed on free accounts. Unfortunately, neither google maps nor sigimera (two APIs we used, among others) are NOT [whitelisted](https://www.pythonanywhere.com/whitelist/), and we didn't know that. Spent a good 30 minutes on those two issues, until AT LAST. 

IT WORKED
---

Totally unexpected. Me and Sohaib were sooo tired (at this point, it was 6:30). But we did it. 

What does this mean?
---
Another facet of our project done, of course. We're gonna have to wait until the end of November to start the actual web work and fixing android app bugs, since we have 314 and 311 tests next week, and then I have MLH prime the week after. Sucks, but these things happen, of course. We hope to have a completed module by around Christmas time, and then we'll start doing user testing! On you guys, of course. Submit it to Detroit Hacks, and then start getting funding for expanding the application. Lots of great things coming up!
