---
author: Randy Bias
comments: true
date: 2008-06-22 08:42:33+00:00
layout: post
slug: cloud-values
title: Cloud Values
wordpress_id: 2354
old_categories:
- Cloud Computing
- Technology
---

If you haven't noticed, the cloud computing conversation is in full swing.  There has been a [vigorous discussion](http://groups.google.com/group/cloud-computing/browse_thread/thread/2387c02a883ae612) recently on both blogs and the [Cloud Computing Group](http://groups.google.com/group/cloud-computing) around defining 'cloud computing' and everyone is taking a swag at it; usually with their own bias.  Of course, I already have my own [bias](http://neotactics.com/blog/technology/short-sighted-about-cloud-computing) (ha!), but Reuven Cohen, CTO of Enomalism, had a recent posting, [Describing Cloud](http://elasticvapor.com/2008/06/describing-cloud.html), that I want to respond to.

**Internet Centric Services**
Reuven uses the notion of 'internet centric software' to describe cloud computing services and talks about a shift happening from a 'single tenant approach to software development' to a 'scalable, multi-tenant, multi-platform, multi-network' approach.  I like the notion of 'internet centric software' and for me, it says much about the fact that the latest boom is one where people are trying to find new Internet-relevant business models rather than trying to move bricks and mortar online.

Calling it 'software' still irks me, though.  Developers aren't consuming software in this new world.  They are consuming cloud services, adding traditional software development, and putting together all new applications that are [greater than the sum of the parts](http://blogs.smugmug.com/don/2008/06/03/skynet-lives-aka-ec2-smugmug/).

**The Real Buzzword**
What really irks me more is the notion that there is one problem: _scale_.  If there is one buzzword that is more useless or more watered down than 'cloud computing', it's got to be so-called 'scale'.  Beyond the fact that it's [misunderstood](http://neotactics.com/blog/technology/auto-magical-scaling/) and treated like a panacea is the fact that it masks a whole set of real, compelling problems and solutions.
<!-- more -->
**On-demand is in Demand**
Let me walk you through this.  Amazon has already told us that the majority of their AWS customers aren't [startups](http://www.techcrunch.com/2008/04/21/who-are-the-biggest-users-of-amazon-web-services-its-not-startups/), but large corporations.  Are large corporations building scalable websites?

No.  They have other needs.  Cloud services value propositions serve both 'scale' and these other needs.

As I see it, the fundamental value props of cloud services are:


  * Scalability
  * Leverage
  * Speed
  * Reach


_Scalability_
Everyone knows this one, so I won't dwell on it too much, except to define it clearly.  Scale is the ability of your resources to service demand.  A scalable site, system, or business is able to manage resources in such a way that it meets the service, product, or consumer demands as they grow.  That's it.  Nothing more.  The trick is that most things, online or off, aren't designed to scale by default.  In the simplest terms, it's your ability to handle the [Slashdot or Digg Effect](http://en.wikipedia.org/wiki/Slashdot_effect).

_Leverage_
This gets lumped in with scalability, but it's not exactly the same thing.  You get leverage when you are able to go from zero to 'lots' quickly, but not necessarily because you have a consumer or other uncontrollable demand.  For example, you might need to crunch a large amount of data periodically or perhaps you need to do 10 test runs of your application deployment simultaneously.  It's a predictable, quantifiable need that is under your control, but now you can get on-demand resources to service that need, where before you couldn't.  I think the majority of greenfield cloud usage is of this type.

_Speed_
Easy:  "I need 10 servers in the next hour to finish this project on time."  I believe this particular use case is extremely prevalent with enterprise customers right now.  There is much less friction in turning on 10 servers on EC2 than trying to get them through corporate IT.  Combined with elasticity, you can get tremendous leverage and significantly reduce time to market or time to complete a project.

_Reach_
This is part of what Reuven was alluding to in the original posting where he says 'global'.  We haven't seen this as much yet, but will soon.  As clouds go global, your ability to more directly reach a given market goes up dramatically.  I like to think about the Friendster case.

Friendster is a U.S. bred-and-born social network; one of the first in fact. It had strong initial traction in the U.S., but was eventually eclipsed by MySpace and Facebook.  Yet, [Friendster is still around](http://en.wikipedia.org/wiki/Friendster), mostly in Asia.  In fact, [39% of it's traffic is from the Philippines](http://newsinfo.inquirer.net/inquirerheadlines/nation/view/20080622-144061/Filipinos-are-prolific-go-and-Multiply).  In a world where clouds are global, it will be easy for a Friendster to shift infrastructure as markets shift, resulting in better service to and huge cost savings in serving those markets.

**Summary**
So what's the punchline?  It's going to take a while for the terms to settle down, but [don't be overly swayed](http://neotactics.com/blog/technology/auto-magical-scaling/) by the 'scalability' proposition.  Not only is scalability not easy to create, but it's not just about scale.  There are some very powerful ways to gain leverage through the elasticity that cloud computing services enable.
