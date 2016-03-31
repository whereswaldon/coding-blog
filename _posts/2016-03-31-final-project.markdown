---
layout: post
title:  "Final Project"
date:   2016-03-30 6:57pm
categories: jekyll update
---

As I mentioned in my last post, viewing CITIZENFOUR
radically altered the way that I perceive security
and inspired me to learn how to do modern encryption
techniques. That has grown into a passion for
encryption in general. As a final class project
(in the class that introduced me to CITIZENFOUR), I'd
like to write a relatively non-technical guide to
achieving strongly-encrypted communication. As per
the instructions of my instructor, I will also
briefly discuss the ethics of such measures, but I
don't know quite what to say. Encryption protects everyone.
I understand that this means that encryption protects
organized crime, but it also protects me from all kinds of
mallicious information-harvesting. It's much like the discussion
surrounding gun law, though much more relevant to my
day-to-day.

Gun advocates say that guns protect people for other people
with guns, and that "guns don't kill people; people kill people."
While I don't have very strong feelings on gun law, I think
a similar metaphor is applicable to encryption. It's not whether
you have it, it's how you use it. A large part of why I want to
encrypt my communications is to protect myself from common
exploits on the internet (such as man-in-the-middle attacks).

This week, something happened to strengthen my convictions about
encrypting the web even further: my roommate's class project
was hacked. Allow me to explain what I mean by that: His project was
a simple informational website that was hosted by a third party and
only supported HTTP. After working on the site for a while, a ton of
strange popups and other oddities began popping up. They rendered the
site unusable, and my roommate consulted me about the problem. When
we looked through the page editors of the platform that he was using,
we found script tags that had been injected to load the third-party
mallicious code. Best as I can tell, this is what happened:

1. He logged in over HTTP
2. Something intercepted the packet and grabbed his plaintext username & password
3. That code crawled the site and injected its code in a couple of places
4. That same mallicious code continued logging in periodically to add more mallicous code

I think it was some kind of script because there was not motive whatsoever to the exploit.
Nobody gained anything from doing this, so it must have been automatic. My roommate has
since had the site secured under HTTPS and has changed his password, so
there shouldn't be any further trouble.

It's crap like this that makes me passionate about encryption. The SSL
that now protects his site protects him and his data from the 
mallicous and technically savvy. In my ideal world, such protection would be taken
for granted, but such a place is a long way off, if it can exist at all.
