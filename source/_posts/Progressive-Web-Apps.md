---
title: Progressive Web Apps
date: 2017-02-12 10:52:46
tags:

  - Morgan
  - Murrah
  - Web Development
  - HTML5
  - Chrome
  - Service Worker
  - Offline-First
  
---

## What's trending? Progressive Web Apps and Offline-first design. 

### (So says I....)

Keeping abreast of new developments is essential to web development. It can also be very draining, as many things come and go at an incredible pace particularly in the realm of JavaScript Frameworks. This can be exhausting and install a certain amount of skepticism in adopting or event really having a look at new things, this is sometimes particularly called *JavaScript Fatigue* as the rate of change has been so dramatic in the last few years. 

Many mentors and experienced people I have talked to have instilled this in me some as well as a virtue to hang back and only invest in the 'proven' technologies. However some new developments really do seem to pass muster and persuade me that they are going to be a huge part of the future of web development. (What follows, of course, is also the sometimes pained realization one must find time to learn this new shiny thing when one is already very busy...).

 Most recently the emerging concepts of **Progressive Web Apps** and **Offline-first design** have caught me and a number of conference talks have persuaded me that I need to become familiar with this technology... for the right reasons.

The following article is excellent and essential introductory reading, with some great visuals:

#### ["The Offline-first Cookbook"](https://developers.google.com/web/fundamentals/instant-and-offline/offline-cookbook/) by Jake Archibald

![](https://developers.google.com/web/fundamentals/instant-and-offline/offline-cookbook/images/cm-on-install-dep.png)



#### I also watched some of the following videos:


<!-- * **Progressive Web Apps with Alex Russell** -->

[![Progressive Web Apps with Alex Russell](https://i.imgur.com/Rzj5u9N.png)](https://www.youtube.com/watch?v=x7cfLDFVyHo "Progressive Web Apps with Alex Russell")

<!-- * **An Introduction to Service Workers - JS Monthly London** -->

[![An Introduction to Service Workers - JS Monthly London](https://i.imgur.com/khlcTF8.png)](https://www.youtube.com/watch?v=EnaKD_EHG14 "An Introduction to Service Workers - JS Monthly London")

<!-- * **The ServiceWorker: The network layer is yours to own** -->

[![The ServiceWorker: The network layer is yours to own](https://i.imgur.com/6F6wduj.png)](https://www.youtube.com/watch?v=4uQMl7mFB6g&t=217s "The ServiceWorker: The network layer is yours to own")


---

# What I believe I learned...


A Progressive Web App is...

[![Progressive Web Apps is the new Ajax - View Source Conference Sep 2016](https://i.imgur.com/Kz3EP6x.png)](https://www.youtube.com/watch?v=EErueQdEXMA " (https://www.youtube.com/watch?v=EErueQdEXMA "Progressive Web Apps is the new Ajax" - View Source Conference talk by Chris Wilson "Progressive Web Apps is the new Ajax")


### **My very junior summary...**:

> 1. **Web Browsers are increasingly sophisticated and advanced to the point that is possible to have 'offline-first' applications that fill all of the UX needs of users currently met by native applications. The idea that the web was dead for mobile does not seem to be certain or bearing out with time**

> 2. **The costs of developing native applications for iOS/Android platforms and others is prohibitive and has documented issues with adoption/attrition (See: Progressive Web Apps w/ Alex Russell). If anything, it is native applications which look ready for 'disruption' from progressive web apps.**
> 
> 3. **JavaScript is undoubtedly at the core of this paradigm shift and meeting users desires for consistent, engaging design.**

You might still be wondering Offline web... WHAT? Well what offline-first really means are web apps that only truly need to load once. From that point a service worker starts from the second load and the app should function gracefully even if you are offline or network connection is spotty. You should not get network unavailable/i.e. the "downasaur" even if you have no internet connection.

![](https://qph.ec.quoracdn.net/main-qimg-2726194a5aea31c692cc6ccb06457469)
**This dinosaur could be becoming extinct if service workers become as standard as they could be...**

'Service Workers' as I understand them from the literature and my early experimenting act as a proxy between you and the network, and are capable in experimental stages of performing many features that native mobile apps provide i.e. push notifications, homescreen icons.

With offline-first applications at a minimum there is never a no internet connection available warning or a hanging spinning loading animation. There now exists a whole plane to "control the network" as Jake Archibald calls it to ensure there is a consistent, smooth experience throughout the app. The project to make a Offline Wikipedia to me is exciting and shows the real potential for offline-first to affect the many.

#### [Pokedex.org](pokedex.org) is an example of an offline-capable website using a serviceworker and database within the browser.

I see a major driver for the future adoption of this offline-first, progressive web app approach is the fact that the resources needed to develop native mobile applications for Android and iOS is more than most organizations have or wish to expend. There are limitations to hybrid mobile app design like using PhoneGap, what I am currently working with on my job, but these hybrid approaches through the appstore could become even more performant with the use of service workers.
