---
title: "Target Credit Card Breach"
date: "2014-01-20T17:31:02-07:00"
slug: "target-credit-card-breach"
aliases: ["/news/2014/1/20/target-credit-card-breach"]
lastmod: "2014-01-20T18:08:10-07:00"
categories: ["Privacy"]
tags: ["Security", "Finance"]
---

The breach of data from Target (along with Neiman Marcus and reportedly a few more) seems to be getting worse by the day. There are some things I find highly concerning.

### First, some facts.

1.  Attacks started on November 27, 2013 (just in time for Black Friday).
2.  The attack went unnoticed until December 15, 2013, over two weeks later.
3.  Hackers got names, addresses, email addresses, and phone numbers of 70 million people; 11GB of data total.
4.  Siphoned data has been sent to Russia and who knows where else from there.
5.  Attackers used a [RAM scraper](http://www.wired.com/threatlevel/2014/01/target-malware-identified/) to capture un-encrypted data from point-of-sale systems after the credit card swipe, but before it was encrypted and sent to a central location for routing to the credit card companies.
6.  Target and Neiman Marcus both passed all annual compliance testing for their handling of credit card data by the credit card industry standard ([PCI-DSS](http://en.wikipedia.org/wiki/Payment_Card_Industry_Data_Security_Standard)).
7.  A [similar attack](http://www.wired.com/threatlevel/2010/03/tjx-sentencing/) happened in 2005.

### Why does this keep happening?

The short answer is pretty simple, as disappointing as it is. The industry standard is subpar, retailers are too cheap to upgrade, and people are frequently reactive in nature. Now there's something to react to, let's see if it works.

So let's break that down. The standards exist, but they're too weak. In fact, these retailers passed their most recent annual inspection, though the post-crisis analysis shows they're no longer in compliance. Seems like a pretty obvious solution - there needs to be constant monitoring for compliance. 

Even constantly being compliant will not suffice though, case and point:

> In August 2006, Wal-Mart was also certified PCI-compliant **while** unknown attackers were lurking on its network. \[Emphases is mine.\]

So what needs to change? Two excerpts caught my eye:

> PCI standards don’t require companies to encrypt card data while in transit either on the company’s internal network or on its way to a processor, as long as the transmission is over a private network.

> Target was likely using such a secure channel within its network to transmit unencrypted card data. But that wasn’t good enough. The attackers simply adapted by employing a RAM scraper to grab the data in the point-of-sale device’s memory, where it was not secured.

To overcome these obstacles, there needs to be an unbiased third party to write the new compliance standard. This new standard needs to be written with the understanding that retailers can and will opt for the *bare minimum* implementation that meets the standard; they have very little incentive to do otherwise (sadly caring for their customers isn't nearly as profitable as appearing to care for their customers). This means adopting the already-circulating [EMV card](http://en.wikipedia.org/wiki/EMV) standard and end-to-end encryption on payment systems. 

There is no silver bullet. It's a general rule of thumb that hackers will always be one step ahead of security. With the right measures in place, we just might be able to catch the leak after 70 credit cards are stolen rather than 70 million. I am also not a security expert, but when flaws are this glaringly obvious people have the right to be outraged.
