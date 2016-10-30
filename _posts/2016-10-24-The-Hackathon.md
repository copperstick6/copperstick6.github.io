---
layout: post
title: First Hackathon and Reflections
---

What's up, what is this? I thought you hate writing anything...
---
A friend of mine told me to create this 'blog' because he thinks that I have too much on my mind all the time, and he thinks I'm slowly deviating from the fun person I usually am, and that I'm becoming a workaholic =S.

Well, I guess he's right.

So... what're you up to?
---
Honestly, the hackathon last week messed up everything in a good and a bad way. Screwed my sleeping patterns for a whole week (Sorry roomie for staying up till 3 AM, totes my bad, I'll buy you lunch tomorrow to make up for it). Other than losing a Saturday and Sunday that I could have used to catch up on work, I guess those are the only ways that the Hackathon really screwed me.

Well, onto the mostly good part, we did win, with our application [SAFE](https://devpost.com/software/hacktx-safe). The application ensures the safety of your surroundings by notifying you via text message or notifications on the app whether anything fishy's going on near you (shootings, burglaries, etc). 

I learned a lot with this hackathon, having to scramble to learn Python and [Flask](http://flask.pocoo.org/) the week before the hackathon, as I had a Data Structues test the week before, and Jane Street the week before that, so it was a collossal mess, and I was in a huuuge rush. At the hackathon, it turned out that my teammates were utilizing Python v3.5, and I was practicing with v2.7, so I had to look up tutorials for the first 2 hours, but in the end it worked out. We spent the first 2 hours hashing out our idea anyways, so productivity was not lost at all, fortunately.

I worked with A LOT of APIs. First, I worked with Twilio, a popular API that allows you to send messages to others automatically, and then I worked with Google Maps API to figure out a way to obtain user location and/or convert that to latitude and longitude coordinates. The Geolocation functionality within the Maps API made that so much easier than it could have been. And finally came all the APIs that contained all the data for shootings, crimes, natural disasters, and the like.

Eventually, I transitioned to working backend with Sohaib, and we spent the entire night figuring out how to run our code from Amazon EC2 and Beanstalk. Let me tell you, it was not fun. Turns out, they don't support many of the flask packages, and they don't support a lot of the functionalities we had. Took us 10 hours to attempt to figure out. When Sohaib fell asleep for a quick 1 hour nap, I went to another buddy who just suggested we just host it off our local machines, because we didn't have much time left (at this point, it was 8:45), and that's what we ended up doing. Never forget the best domain ever: turtleboys.com. Thanks to zach for owning that domain already haha.

Our android guys, meanwhile, were working the android app. They did a great job, really pleased with what they came up with. They created an elegant solution to run our scripts via their app while we were tinkering, and that's what we ended up using.

After everyone figured out the backend problems and such, I just focused on writing the DevPost, and creating what would eventually form the basis of the Amazon Alexa project. It was just 4 hours of me figuring out the documentation and attempting to hobble together a solution, before realizing that my [intents](https://github.com/copperstick6/HackTX-SAFE/blob/master/intent.json) were all screwed up and I had to go back and fix it again. Not fun at all. So I created a half finished solution that I just sucked up 4 hours and didn't really contribute anything to the project. That made me kinda salty =l.

Well, after noon hit, I basically half slept, half walked through the entire day. Not very fun tbh. My throat was sore and my nose was runny, but I struggled through presentations. I was sooo exhausted that I just crashed into bed and fell asleep the moment I touched the bed.

After I kinda woke up at 12 the next day, I realized the feasibility and possible marketability of our creation, and well, we're going to continue to develop it. We plan to submit a completed version to [goDetroit](https://godetroit.devpost.com/?ref_content=featured&ref_feature=challenge&ref_medium=discover) and possible make it a freemium app with lots of features. 

I guess that's kinda it. I still gotta prepare for MLH Prime in 3 weeks. I plan to learn some Node.js to prepare for the hackathon, as a lot of API calls can be simplified using Node. I was using string concatenation to make a custom URL to get the url data beforehadn in Python. Super inefficient. I plan on learning Node.js just to increase my efficieny and increase what I can do.
