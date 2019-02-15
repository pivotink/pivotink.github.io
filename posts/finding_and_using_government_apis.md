---
layout: post 
title:  "Finding and using Government APIs"
subtitle: "We're working with all levels of government to collect and document government APIs and other machine-to-machine services in one place."
date:   2019-02-15
---


## A brief history of common approaches to Government APIs

It's not the first time we've tried this.

Standard Business Reporting [SBR](http://sbr.gov.au), a whole of government initiative to reduce the burden on businesses in their dealings with government, went live almost 10 years ago. 

SBR brought people together across government who wanted to replace paper forms with data exchanges. Underpinning this goal was the belief that a standard set of technologies would lower costs for everyone. 

Fast forward 10 years, and we've now discovered that one-size doesn't fit-all.

Although the program has been quite successful, the chosen technologies weren't suitable for a wide range of data exchanges.
New agencies have also had difficulty adopting the technologies, limiting the benefits to a small percentage of the total number of interactions.

It would be all too easy to blame the technology; to suggest that others would have worked better.

But the truth is:
 - We've learned that different communities do things differently, and for good reason
 - Some things should be standardised for everyone, but others should be left to individual communities to choose for themselves
 - And most importantly, no one set of standards could possibly be suitable for all the digital interactions in Australia


More than ever, Australians (as individuals or businesses) are interacting digitally with government. There is as much need to reduce their burden in dealing digitally with government now, as there was almost 10 years ago.

We at don't want to lose the good things about standardisation, but we also know more now about what works, and what doesn't.

## Doubling down on API discovery

{: .post__content--right}
![Screenshot of api.gov.au showing the description of an api](/img/Definitions_Catalogue___api_gov_au.png)

One thing that we know (and through user research, have reconfirmed) is that everyone benefits from advertising government APIs in the one place. 
So that's what we're doing: Building a platform to catalogue and discover the APIs that are made available by all levels of the Australian Government.

It's called [api.gov.au](https://api.gov.au)

Our team works with all levels of government to collect and document government APIs and other machine-to-machine services in one place.

We're designing the platform to not only be the place where APIs are discovered, but helps authors write better and more consistent documentation. Our hypothesis is that this will make it much easier for people looking to consume apis to pick and choose the right one for them.

> **It's important to note:** when we say 'api' we mean any technology that lets two systems interact and exchange data. While we have a preference for RESTfully designed JSON apis, we don't care if the technology is SOAP, WS\* or even SFTP. If lets people better exchange digital data with government, we'll take it.


## Good data definitions are just as important

{: .post__content--left}
![Screenshot of api.gov.au showing a data definition](/img/Definitions_Catalogue.png)

We also built the [Definitions Catalogue](https://api.gov.au/definitions), the place where Government defines it's digital data.

Here, anyone can find the data definitions used by Government on their APIs. This helps Government not only share data more effecitvely, but they can standardise on the information they collect from others, reducing duplicate reporting and double handling.

A key feature we discovered through research is that not everyone in Government calls a spade a spade. We know that in SBR there duplicate definitions exist for the simple reason that people found it too hard to search if a definition already existed.

To combat this we've introduced the ability to include synonyms in your search, meaning if you search for 'spade' we'll also search 'shovel'. But that's not enough to make sure people find what they're after.

We've also got the capability to show you related definitions, so if in your quest for the perfect gardening tool, once you've found spades, we can also show you rakes. 

Here's an example:

{: .post__content--full}
![An image showing the definitions related to location](https://api.gov.au/graph/relations.png?url=https://api.gov.au/definitions/api/definition/ce/ce52)

### Sharing your definitions in the catalogue
If you want to share some of your definitions in the catalogue, we've put together a quick and dirty tool to help while we're building something propper.

You'll need to prepare a CSV file with one row per definition, with separate coluns for:
 - Name
 - Definition

That's the bare minimum, but we'll also take:
- Guidance
- A unique identifier
- It's datatype
- It's status (published, draft, etc)

You can find the definitions ingester [here](https://definitions-ingester.herokuapp.com/)

## Sharing what we know 

{: .post__content--right}
![Screenshot of a table describing the supported features of various technologies](/img/Digital_Community_Playbook.png)

We're also working on what we're calling the [Digital Community Playbook](https://api.gov.au/playbook), a collection of best-practice guides for government, by government, on how to do better digital data exchange.

We've tried to think about things from every angle, not just technology.

In the playbook you'll find guides on imporant topics like choosing a governance model, how to document your decisions, and how to consult with your community.

We're going to start collecting feedback from both api.gov.au and the definitions catalogue to see what works, and what doesn't, and including this in the playbook over time.

> **It's important to note:** We don't claim to be the experts at this, but we didn't want to start with a blank page. If you find something that we've written that is ambigious, misleading or just plain wrong, let us know and we'll make it better together.


## We're all in this togeher

We've also setup an [open community](https://api.gov.au/community/) for anyone in governemt who uses, creates, or has an interest in APIs to get together and share information.

Even if we don't end up listing your APIs on our catalogue, or sharing your defintions, we can still learn from and help eachother. 

If you would like to get involved, or just learn more about what we're doing and why, don't be shy. Reach out.


## Under the hood

Everything we’re working on is open source and available at our [github repository](https://github.com/apigovau). 

It's a little out of date, but here are some more techincal or detailed images that you might find interesting:


### Our product roadmap 

{: .post__content--full}
![An image showing the major components of upcomming work for api.gov.au](/img/roadmap.png)

### The technology and microservices

{: .post__content--full}
![An image showing the technology and microservices of api.gov.au](/img/architecure.png)

### Our 'Virtuous Cycle' 

{: .post__content--full}
![An image showing how getting more users will help get feedback, which will help build better services, which will get more users](/img/growth.png)

### The semantic relationships in the Definitions Catalogue  

{: .post__content--full}
![An image showing the types of relationships that will be shown in the definitions catalgoue](/img/Semantic Relations.png)
