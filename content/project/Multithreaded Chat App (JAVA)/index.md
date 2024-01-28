---
title: Multithreaded Chat App 
summary: A chat application written in JAVA which leverages parallel processing of threads.
tags:
  - Software 
date: '2020-12-27T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: Chat App
  focal_point: Smart

# links:
#   - icon: twitter
#     icon_pack: fab
#     name: Follow
#     url: https://twitter.com/georgecushen
url_code: 'https://github.com/alifelham/Multithreaded-Chat-App'
url_pdf: ''
url_slides: ''
url_video: ''

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
# slides: example
---

This is a software which can be used by three users to have a conversation from a single device. One user can address a message to another user using the '@' character and the software will automatically ask that user to answer to the message. The user is also allowed to leave the chat by typing "stop".

# Description of the program code:

The chatDriver class creates an object 'm' of the chatThread class. It passes the object to the constructors of chatT1, chatT2, and chatT3 classes at the time of creating class instances of these respective classes. The constructors of chatT1, chatT2, and chatT3 receive an object of chatThread class as its parameter and then sets it as its own copy of the object by using this.m = m1, this.m = m2, this.m = m3 respectively. The constructors also start the thread blocks. The thread blocks are within the run( ) blocks inside these classes. Inside each run( ) method's scope is a while loop which runs as long as the threads are not interrupted. If they are interrupted then it shows in the screen that a certain user has left the conversation. It checks if more than one users are left or not. If more than one users are left then the control is passed to another thread. The chatThread class has three important methods named speakerA, speakerB, and speakerC all of which are synchronized threads. All of them also throw InterruptedException handled by their caller methods. There is a String variable named flag which is used to set the speaker of the conversation. An int variable named user sets the number of users. Each speakerName method checks if the flag is set to that speaker's name. If it is not then the thread is made to wait. If it is set to that speaker's name then the methods takes an input from the user. If the input is "stop" then the thread is interrupted and control is passed to another thread.

All cases and spaces are ignored. If the message is not "stop" then the message is parsed in two parts. The part before the "@" character is the message and the latter part is the name of the user it is addressed to. The cases and spaces are ignored here as well. The flag variable is then set to that name and the other threads are notified. All these classes work hand in hand to carry out the conversation between the three users until two of them have typed "stop".
