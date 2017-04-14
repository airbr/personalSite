---
title: Classified - Give your a website a Free Service Worker
date: 2017-04-14 14:07:16
tags:
---

Intended for a general Atlanta/ Switchyards Downtown Club audience...


**Banish the Fail T-Rex: Making your website offline capable so that users never or see less of the failed internet connection messages.**

![](https://i.imgur.com/j9MIbi6.png)


When the connection goes down, your website or brand doesn't have to (completely). Its a lost opportunity to at least give a parting message/direct the user on how to reconnect with you or your brand. Thing that work offline is classically one main reason people people are drawn to using installed apps over web based services- it helps at least to close the gap.

With the use of some relatively simple but quite new features in web development there is now more capability to handle offline events smoothly using [''Service Workers'" that run outside of the main thread of the browser](https://developers.google.com/web/fundamentals/getting-started/primers/service-workers).

At their most advanced (this isn't really in practice many places yet) service workers can enable almost native app-like experiences, where the user of the website is never aware they have lost connection or are reliant on a connection, because the service worker based development is advanced enough at handling user interaction until the connection is back.

At a very basic level I should be able to enable a static page your website that is served to any user that visits the webpage again when offline. You can make this offline landing page custom to your needs. That is kind of cool, and might genuinely reach some of your users where otherwise the t rex would.

You can visit my website at https://morganwebdev.com where I have a very basic service worker installed that handles offline status by presenting a basic 'empty phone screen' telling the user they are online and call my cell phone. (This website gets a 100/100 on the Lighthouse Audit, btw).


Interested? e: morgan@morganwebdev.com

Ill need from you:

* Access to some source files of like your website logo, and at the very minimum a tree of all of the files in your project and ability to edit your main index.html to make the changes I need, and add new files to your project
   * I could work from a branch of your git, ideally
* (I will let you deploy the changes, or help if its simple)

What I will try and do:

* Set up the most generic service worker possible that handles offline events by service a particular page of your choosing.

   * ++ I could also add some relevant items such as to the manifest.json to enable the website to be saved to a users home screen on mobile devices, to improve your functionality as a Progressive Web App

What I want:

* To get some experience implementing service workers across different projects and making them 'offline capable'. I can't guarantee it will work. It might be hard. I actually have little idea right now.
* Use a screenshot of the offline landing page from your startup/website as part of a portfolio collection if it is working.

Also:
*  No warranties