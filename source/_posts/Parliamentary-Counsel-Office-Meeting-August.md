---
title: 'Parliamentary Counsel Office Meeting, August'
tags:

  - Legolas
  - GovHack
  - New Zealand
  - Legislation
  - Lawyer
  - Law Reform
  - Code
  - Law
  - Murrah
  - Parliamentary Counsel Office
  - XML
  - HTML
  - API
  - XSLT
  - Open Data
  - Hackathon
  - Github
  - Drupal
  - PCO
  - General Assembly
  - Atlanta
permalink: parliamentary-counsel-office-meeting-august
id: 34
updated: '2016-08-22 15:36:36'
date: 2016-08-18 18:37:37
---

Project [Legolas.nz](legolas.nz)

---
#####**A quick recap**
In case I haven't told you already... 

It was great to read about the [2016 GovHack](https://www.govhack.org/) going smoothly. Unfortunately it was not practicable for me to attend on US Eastern time but not for a lack of trying! ('16 hours behind' is pretty off the beat!). [In 2015 I was proud to be part of a team that won the first national spirit of GovHack award. We were also representing New Zealand in Australia in the first GovHack Awards where the official competition included New Zealand.](https://www.odt.co.nz/news/dunedin/dunedin-website-team-wins-nationwide-competition)

Like anything else you could make in 46 hours, our project result from 2015 is still a humble looking project. However, it achieved an important proof-of-concept: a first initial set of features that received a warm response from the community and recognition of the Judges of Govhack 2015.

> Everything you see at legolas.nz was made in 46 hours, maybe with a few typos fixed later. Our project video was made with freemium software that retains an audio watermark in the background. Its all kinda naff like most hacked together things.

This was accomplished with special credit to [Chris Burgess](https://github.com/xurizaemon) who used the .XML dataset with no access to a corresponding .XSLT stylesheet at the time and still produced what you see at [legolas.nz](). That is, the entire set of legislation from 2015 displayed in a (roughly) visually similar appearance with the ability for inline comments, styled using some basic reverse engineering. This set of legislation is searchable and commentable.

>That this is even possible is pretty special when you consider the pace of change in this area[^1]:

* **1267 AD - [Statute of Marlborough c.23](http://legislation.govt.nz/subscribe/act/imperial/1267/0023/1.0)**
The oldest piece of statute law not repealed in the UK. Still contained within the NZ Imperial statute books still and in the [XML Dataset](http://legislation.govt.nz/subscribe/act/imperial/1267/0023/1.0/096be8ed8009afe5.xml).
* **2002 AD - [New Zealand Legislation goes online](https://www.beehive.govt.nz/release/new-zealand-legislation-goes-line)**
* **2015 AD - [New Zealand Legislation in PDF gains official version status](https://gazette.govt.nz/notice/id/2014-ps71)**
* **2016 AD - [New Zealand Legislation in HTML gains official version status](https://gazette.govt.nz/notice/id/2015-ps7126)**

#### Why is HTML becoming an [official version](http://www.legislation.govt.nz/act/public/2012/0119/latest/DLM2998516.html?search=ts_act%40bill%40regulation%40deemedreg_legislation+2012_resel_25_a&p=1) significant?
<br>

I imagine there must have been some reasons for the PCO to make the change in the first place. For those wanting concrete examples:

##### At Court

> In a courtroom, a lawyer could use a device such as an tablet or laptop to display the official HTML or PDF version from the NZ Legislation website and this would be recognized as displaying an official source of legislation (by legislation). 

It might seem trivial but it could save some weight of carrying redundant copies of legislation. Maybe a lawyer forgot something and the digital official version is a handy substitute. Many lawyers can't do this in other places.

> In a courtroom, a self-represented party in a case could cite legislation that they discovered by googling on their device before or during the case. 

Which I think is good. More time for discussing relevance, less time on the officiousness around materials being presented. Someone insisting on self-representing is facing an uphill battle as-is. People are going to be an 'internet lawyer' despite all warnings not to and we can really only hope to increase the quality of what they access. 

[Lawyers or Pro Se in another jurisdictions for example would have to cite only from a printed official annotated code from that jurisdiction that costs several hundred dollars.](http://www.lexisnexis.com/hottopics/gacode/Default.asp)

##### Digital futures

Much less concrete but more exciting has been our groups discussions on what things like this could mean for the future of legislation and ways people interact with it.

**Meeting**
--
The award from Govhack 2015 and attending the wonderful GovHack Red Carpet awards at the Powerhouse Museum in Sydney left us with a lot questions and excitement. This is another way of saying, development stopped for the time being. We knew we had to talk to the PCO before we invested more time before and making any false start either, given our experience not having the stylesheet.

We recently conferenced with two staff of the PCO, Richard Wallace and Michelle Groves. Both had great information and some directing questions for our project. We appreciate their time and the PCO had some good directive our project needed a better scope. We were also reminded of the specific neutral role of the PCO and limitations on help the PCO could provide.

Scope is key for any software. *My stab at a definition is:*

> a free and open source software project to enable independent annotation, visualization and data science on the datasets of New Zealand legislative instruments **<small>with the requirement of preserving the integrity of the underlying legislative instrument and/or its official legal status within New Zealand</small>**

We think that such a project could help enable a whole variety of other projects in the public interest and generally increase readership and engagement with legislative sources in their best data forms. Consder it "Ctrl-f" rather than "Our political solution: manifesto V1.0". Think more ["Single Source of Truth"](https://en.wikipedia.org/wiki/Single_source_of_truth) rather than something more literal in a political sphere. I imagine it would easily be able to be forked for other jurisdictions.

In our particular concept we used the example of inline comments, but that was just one potential application, with other loose ideas floated as user stories to consider further.

We believe alongside this technical scope that tools meeting the purpose we describe above could help improve the quality of debate in our democracy. This is our opinion, and we shared some thoughts about this in our GovHack project, but they are not ipso facto what we set out to accomplish.

I don't think it is splitting hairs to say we may have our own personal political opinions but wish to work on a tool that could be usable by someone of a different opinion. I think it is motivating and would hope to prove something by making a good tool. 


The above reasons are why I think it could be a good collaborative open-source project. There are some notable ones where different 'interests' such as the [Jupyter Project](https://jupyter.org/) which combines elements of finance and science, the [Tor Project](https://www.torproject.org/) which combines NGO and Human Rights support as well as support by various Governmental bodies such as US Federal Agencies.

We certainly don't expect superior access to data over anyone else. What we want, with some co-operation, is a "better API" for interfacing with the PCO. [That governance needs a better API is a little bit of a rallying call from GovHack.](https://www.dto.gov.au/blog/hacking-for-better-government-services/)

**Future**
--
I suggested in the conference that there are particular features to New Zealand legislation that make it appropriate to develop such particular tools. Development since the weekend so far has been in the form of planning and discussion, also engaging with materials such as the New Zealand Law Style Guide and developments in legislation.

So what do I mean? First, we should assess what the status quo is. [Credit where credit is due: NZ is ahead of the curve on this particular issue and in general](https://en.wikipedia.org/wiki/Digital_5). Which is great.

###### Technical 

![](http://www.lawfoundation.org.nz/style-guide/images/nzlsg_cover.jpg)

[XML Dataset details from the PCO were posted  ](https://data.govt.nz/dataset/show/776)as part of GovHack to give access to the online file structure. 

These directories are public but this information about the file structure allows for greater ease finding and copying material. This is one kind of API- giving practical details of how to interact with a dataset.

One issue though is that usually a stylesheet in XSLT format to render the XML into the HTML legislation you see on the website, unless the PCO uses some specific XML conversion software that does not require it. 

> A snippet of NZ legislation dataset in .XML:
```
<?xml version='1.0' encoding='UTF-8'?>
<act date.assent="" id="DLM10900" in.amend="false" xml:lang="en-NZ" irdnumbering="no" act.no="23" act.type="imperial" date.as.at="2007-09-03" date.first.valid="2007-09-18" stage="reprint" year="1267"><cover id="DLM10901"><title xml:lang="en-NZ">Statute of Marlborough 1267</title><cover.reprint-note><para xml:lang="en-NZ"></para><admin-office>Source: New Zealand Parliamentary Library, International Documents Collection</admin-office></cover.reprint-note></cover>
```


There are also some technical matters such as the semantic labelling of HTML elements in NZ Legislation that are not obvious with internal documentation.

We have had some initial communication following the meeting, suggesting to use the minified CSS with the HTML, but we are planning to follow up with more queries about the formatting from .XML as it will likely be the best way to rendering HTML pages on our own platform.

PDF's are by nature just a set of digital images layered onto each other. Its exactly for the reason they are great for other things they are awful for our purposes. PDF's are great if you do not want to accidentally ruin the formatting of/edit. PDF's are unsuitable for this project, which calls for a degree of flexibility and ability to edit to separate concerns of the software applying onto the legislation. 


---

... and there is an update. Some 1400 words. But hey, our Democracy and its laws are interesting enough. Lets keep this conversation going ^_^.

[As my schedule dictates](https://www.airbridge.ac.nz/2016/08/01/my-schedule-for-the-next-few-months/) I plan to begin personally committing (or making 'pull requests' more like) to try and parse out the text for re-use. 

B Murrah


--

1 -[The Global Development of Free Access to Legal Information](http://papers.ssrn.com/sol3/papers.cfm?abstract_id=1617808)