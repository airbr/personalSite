---
title: Python Bootcamp Recap
tags: |-

  - Web Development
  - Morgan Murrah
  - Atlanta
  - General Assembly
  - Python
  - Bootcamp
  - Coding
  - Development
  - Open Data
  - New Zealand
  - GovHack
  - Legislation
  - Jupyter
  - Cloud
permalink: 1-day-python-bootcamp-recap
id: 36
updated: '2016-08-28 14:04:37'
date: 2016-08-28 11:20:50
---

![Python Logo](https://www.python.org/static/community_logos/python-logo-master-v3-TM.png)
[Fundamentals of Python Bootcamp](https://generalassemb.ly/education/fundamentals-of-python-bootcamp/atlanta)

On Saturday 27th August 2016 I attended the Python Bootcamp at General Assembly in Atlanta in addition to my [regular course studies there](https://www.airbridge.ac.nz/2016/08/01/my-schedule-for-the-next-few-months/). As a current full-time student part of our tuition is effectively in-house credit for the [pretty wide range of workshops/events GA hosts](https://generalassemb.ly/education?).

I decided to attend for two reasons:


* Python is not taught in the Immersive Web Development curriculum

* I knew Python has wide usage in particular fields and is a common 'first language' learned 

  * Python is used by students in the Data Immersive program at General Assembly and I had conversations with some of them about their experiences with Python. My prior exposure to it was mainly from my peers at Otago University who were studying science. Research scientists are a large user group of python.


Walking into this bootcamp there were a number of positive/negative ideas which had been shared to me and I wasn't really informed enough to have an opinion on:

* That Python was elegant and easier than other languages (indeed to the point it could spoil you against learning harder languages)

* That Python was slow and 'bloated' and the reason for its adoption is really just the ease of use that overrides most performance concerns

 * However, there is a related argument/point that in fields such as data science and analytics human resources such as developer time are more scarce than processing power. Hence, sometimes it would be better to have a 'slow program' that produces the right result than one that requires more intensive developer time. This point was explicitly made by the instructor as a rationale for using Python despite its performance issues.

**Format of the bootcamp:**

The Bootcamp went from 10-4pm with a lunch break. It was taught at a fast pace but with opportunities to catch up as the instructor took time to move around the room to help fix any bugs/installation errors. It was assuring to hear the instructor state getting the development environment set up properly is always the biggest challenge in a classroom environment for coding.

To fix part of this problem we used a cloud-based deployment using [C9](www.c9.io) of a [Jupyter](https://jupyter.org/) notebook to view the Python based course materials. This was to enable the python code in the notebook to be run by computers in the cloud and not be reliant on local internet signal quality. 

Nice little starter command:

``jupyter notebook --ip=0.0.0.0 --port=8080 --no-browser``

**Cliff notes:**

* I really liked [Jupyter](https://jupyter.org/). I can see its immediate value in being able to visualize data and 'show your work' with chunks of code leading into that visualization on the same page.

* After the first hour of setting up software and the cloud dev environment we got pretty much straight into it with the basics. A copy of my very first Python code/hello world::

```
>>> import numpy as np
>>> print 'Hello World!!'
Hello World!!
>>> 2+2
4
>>>
```
* We went through major features and aspects of Python vis-a-vis other languages and its quirks. Some interesting ones were:
 *  Python is dynamically typed language, meaning it executes many things on runtime rather than could be executed during compilation. This can cause various side effects and errors. As one resource put it "if a program is statically typed, you know that certain types of errors are not possible".
 * Python has a large version split between user bases of 2.7 and 3.x , and that 2.7 requires a floating point in division is one of the first 'gotchas' associated with Python:

**A 'Gotcha':**
--

**In Python 2.7 you may need to add a floating point for numbers to get have decimal usage or else you get some crazy errors/bugs.... this is 'fixed in Python 3.x:**

**3/2 in Python 2.7:**
```
x = 3
y = 2
print(x/y)
...
Out: 1
```
Wha?

**3/2 in Python 3.x:**
```
x = 3
y = 2
print(x/y)
...
Out: 1.5
```
**To get the more correct 3/2 in Python 2.7...**
```
x = 3
y = 2
print(x*1.0/y)
...
Out: 1.5 
```
I can see how some of these apparently tiny but fundamental changes could make things break...

In the class we touched on a lot in the class including usage of type, control flow, modules. Hard to cover it all here.

**Pretty visualization from near the end of class using Pandas:**
![Python Visualization using Pandas](https://i.imgur.com/n1exROn.png)


Features of Python code
--

**Elegance - Consider the Python For Loop compared to [vanilla Javascript:](http://www.w3schools.com/js/js_loop_for.asp)**

>This:
```
# Measure some strings:
words = ['foo', 'window', 'bar', 'hugewordlengthtester', 'hugewordlengthtesterhugewordlengthtester']
for w in words:
    print w, len(w)
    
words_length = [len(w) for w in words]
```
nb '# ' is the syntax for comments in Python
>Outputs this:

```
foo 3
window 6
bar 3
hugewordlengthtester 20
hugewordlengthtesterhugewordlengthtester 40
```
I barely need to tell _anyone_ who has been anywhere near a [Javascript For Loop](http://www.w3schools.com/js/js_loop_for.asp) that this is a much more elegant and simple code for this function. You can even get it down to 1-2 lines. Credit where credit is due.


**Modules - i.e. Pandas for visualization we saw in class.**

In Python we learned that modules really are just blocks of python that will be 'pre-run' in your terminal, introducing variables and so forth. They are not asynchronous/dynamically updating modules. 

In simple terms this means anytime an update is made to a module a fresh instance of Python is required with that module imported with its incorporated changes.

Even just with the basic importing of Pandas however it was clear how much added functionality became possible for complex visualizations.

**Potential application in my open source project:**

 * **Parsing XML**

  * One issue I am considering closely is XML of NZ Legislation as part of an open-source project. It seems Python has some excellent XML parsing libraries that could prove useful for me.  

Conclusion 
--
Python seems a good option for some of my project ideas and I understand why it is widely used in various applications.

The workflow of python applies well to preparing some kind of program, analysis or visualization and having a chance to leave it to process even overnight, later having a chance to tweak it or edit it the following morning, and deliver it to meet a 5pm deadline. You can produce powerful, high quality work- but it takes place within some boundaries.

This workflow does not seem apply as well to a dynamic, live, web development environment where latency in general should not exceed three seconds. This challenge is heightened as some web applications should be able to meet the needs of potentially millions of users at an 'enterprise' level.

For this reason, learning a little bit of Python was great but re-affirmed the need to eventually learn some statically typed language such as C# to understand the 'other side' of computing where there is a lot more done up front by the developer to prevent performance issues that make up the bigger web applications of today.

It still seems there is some truth to the idea that if things are easier there is usually some drawback somewhere for some purpose. But that is pretty vague too and shouldn't let you get in the way of using the fun and easier tool if its appropriate! 

Anyways, a good introduction to Python!
