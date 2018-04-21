+++
date = "2018-04-21T22:50:33+05:30"
draft = false
title = "The State of Virtual Assistants: Where's the AI?"

+++
A commentary on virtual assistants in 2018 and the future.
<!--more-->

## Background
Given the recent developments in speech recognition and NLP combined with the power of mobile and cloud from the last decade, the development of virtual assistants is not surprising. Assistants are already available across most devices with the services being offered by all the major technology companies. In this post, I will try to summarize what the existing virtual assistant scenario looks like and then offer a view on possible ways to think about the future of this technology. So let’s get started.

## What currently works
### Voice
The most common and intuitive way of interacting with assistants is through voice and with advancements in deep learning, speech to text works quite well. While speech recognition for mixed languages doesn’t work that well today (which would be a very useful addition for countries like India), the lack of it isn’t a deal breaker. There are also ongoing research efforts towards natural sounding text-to-speech engines which is again a welcome change but not really a crucial factor towards the utility of assistants. Voice identification also works reasonably well allowing one end device to be used by multiple people.

### Basic Tasks
In terms of utility provided by assistants, there are basic things that work really well, allowing assistants to be on different devices - reminders, to-do lists, calls, calendars, pre-defined routines for fixed commands, smart-home integration, playing content, and getting answers from the web.

### Apps
There has been a lot of focus recently to allow applications to integrate with assistants to accomplish app-specific tasks - like getting an Uber. This allows developers to enable an assistant for their app without solving the speech and NLP issues and at the same time enhancing the “skills” of the assistant.

## Issues
### No Language Understanding
Currently, for almost all production level assistants even the basic tasks as mentioned above work on a pre-defined sentence structure and there is no strong notion of language understanding. Let’s take an example - To send a message, the pre-defined sentence structure looks like “send a message to \<person name\>, \<your message here\>”. The intent is sending a message which the NLP engine can pick up with the keyword “message”. A sentence like “check with \<person name\> what he is up to” is still something the assistants are unable to process. This indicates that we need to work more towards concrete natural language understanding where we are able to parse queries with the same intent but a different sentence structure.

### Engineering
Not all issues with assistants today need AI advancements. A lot of them can be addressed just by good engineering. Let me illustrate this by an example - Google Now does a really good job at recommending commute times based on the calendar and the traffic pattern. It can pick up a table reservation entry from the calendar and give a notification about when to leave for the restaurant based on the commute pattern. However, if you ask the Google Assistant “How does my commute look like?”, it responds with the commute from home to work. What we see here is AI not being the bottleneck - it was possible in this case to figure out the context but it is yet not integrated into the assistant and is purely an engineering issue.

### App Referencing
Currently, each app needs to be enabled or installed on the assistant for the app-specific commands to function. For the enabled apps, there is usually a unique keyword (usually the app name) in the query that triggers a particular app. “Book a cab” doesn’t work, you have to say “Book an Uber” even if Uber is the only enabled ride app on the assistant. Such a flat referencing scheme for each app is not scalable using a voice interface.

## The Way Forward
### Context Awareness and Proactivity
Most assistants currently are reactive and take actions on giving a command. To make them more useful, I think a proactive approach based on complete context awareness might be better. For example - meetings and reminders should be automatically added or removed once detected during a chat with another person. The smart speaker should notify when to leave for office based the daily commute pattern and current traffic instead of the user asking for it every morning. The smart-home evening setting should automatically trigger when the phone’s location indicates arrival at home.

### Bridging the Ecosystem Gap
Currently, assistants are built to work well in a given company’s product suite - you can ask Alexa a question about the movie you are watching on Prime Video or ask Cortana to open a file on OneDrive for you. While this makes business sense, it doesn’t add the most value for the users. I might be using PowerPoint and OneDrive in office and Google Slides and Drive at home. An ideal assistant should be able to respond correctly to the command “open my most recent presentation”. Users will always use multiple services according to their preferences and context from all apps collectively builds the correct context for the user. It is very important for each ecosystem to be able to share context and state with another if you want to put users first. This brings me to my next point.

### Cross-App Decisions and Preference Understanding
If all apps on the assistant share context and state, it opens up the opportunity of making decisions across apps based on user behavior and preferences. The assistant should be able to figure out your favorite food app next time you want to “order Mexican food”. It should understand that you prefer Uber over Lyft unless Lyft is substantially cheaper for that trip and responds to “get me a cab” accordingly. This involves triggering the apps on the assistant which can satisfy the query and then recommending result from the one which has the maximum “utility score” for the user based on previous behavior and preferences and the current context. This also solves the “flat” app referencing issue discussed in the previous section.

## Conclusion
Assistants today are good at defined actions. I believe there is a lot of value virtual assistants can create by making context-aware and personalized intelligent decisions. Let me know what you think in the comment section.
