---
layout: post
title: Fixing the Orthopaedic Surgery Match - A Proposal
subtitle: It's not brain surgery. 
image: /img/aoa.jpg
tags: [The Match, Ortho, Program Directors, programming]
comments: true
---

Two weeks ago ScienceBasedMedicine published my latest post [The Residency Match is Broken](https://sciencebasedmedicine.org/the-residency-match-is-broken/) where I talked about how application fever breaks the match. The only real solution to the problems with the match is a strict limit on the number of applications applicants can send per cycle. Convincing applicants of this is a lost cause, and I don't even bother trying to explain in that article why application caps would work for applicants. I also offer to develop an application cap service for free, so long as people are interested. In this post I want to make the pitch to orthopaedic surgery programs, that this is something that can work, I can pull it off, and that program directors really should entrust the match to a random premed on the internet.
 
So if you're a orthopaedic surgery director, I have a quick few questions I would like to ask you: 

Are you happy with the current state of the residency match? 

Is the large volume of applications you receive a problem for you? 

Are you concerned about the fairness of the application process as it relates to the cost to applicants? 

Do you have trouble telling which applicants are legimately interested in coming to your program? 

If you answered yes to the last 3 questions, you might want to read to the end and see if this is something you're interested in. Application caps would address a lot of these issues and more for you. The large volume of applications is addressed by applicants not being able to send so many applications. With a sane application cap, applicants will be spending less than 200$ in ERAS fees instead of $1500. Finally, because applicants have a limited number of applications you can tell they're interested in coming to your program because they chose to apply to your program. 

There's just one problem, the only group with the power to instantiate application caps in ERAS is the AAMC. The AAMC isn't going to do that, because it would be financially disasterous. Except that isn't technically true, because there is a group that has absolute power to decide what their program does for their recruitment process: individual program directors. Yes, you, the individual program director can decide to have application caps if you want. You just need a couple other program directors to want them too. 

So long as you have a pool of programs of sufficient size and diversity, you can have application caps very easily. All you would need is to develop a website where applicants sign-up and get tokens that they use to apply to programs. This would basically be the same as preference signaling sites that other specialties have used, except its a requirement. This would drastically reduce your application volume, and solve a lot of issues for you and applicants. It would save you and applicants a lot of money. So allow me to prove out how all of this is possible, would work, and basically can't fail. 

## This is Feasible

This is very easy to develop, and very easy to make a successful project. You can learn everything you need to know to build this thing in any web programming textbook. This is the most simple project you can imagine. We're not storing any sensitive user info, we have a low number of users, the interaction models are unsophisticated, and we're not processing payments. There are only 150 programs and less than 1000 applicants meaning this service will run on a single web server. We don't have to worry about load balancing, or the load in general. 

Applicants really want to sign-up and use this system. If you say that you won't consider applications unless applicants do x, y, or z; best believe they're probably going to do whatever x, y, or z is. I don't think there's any chance applicants are just gonna say "screw it" and not applying to the participating programs like what happens with secondary essays. All applicants should want to apply to participating programs because they get the highest return on investment per application by applying to participating programs. If this service is done right, applying to one participating program would improve your chances of matching the same as applying to 3 to 5 non-participating programs. All for the low, low cost of signing up to a website and clicking some checkboxes. 

It will also be very easy for program directors to work with this system. All you have to do is export your data from ERAS with ERAS_ID's, download the data from the application cap website, and filter applications on ERASID. Just lowering the volume of applications you're receiving will solve most of your issues with the application process. Once again I really can't put it into words how easy it is to get this done. If this is what program directors really want, I can have this done before ERAS allows applicants to start sending applications on September 1st at the latest. I would hopefully have it done, validated and ready to go long before then. So a question you might have is: are there any risks? 

## Low/No Risk

I've specifically thought this proposal out to be as low risk and have as many outs as possible, to the point where the risks are basically zero. The two biggest risks are someone hacking the website, and a significant number of programs going unmatched. As for being hacked, the hopefully won't happen because I will use programming best practices, and nobody really has any motivation to hack the site. There's nothing really of value being stored in the database. 

As for programs going unmatched, I don't see this as a big risk because we can communicate with applicants about what we're doing, we can easily identify programs that are at risk of going unmatched, and we have the tools to make whatever course corrections are necessary. We aren't changing anything significant about the match: you're still accepting and reviewing applications through ERAS, and sending your rank list to the NRMP. As a result, all of the data from the NRMP can be used to predict what the results will be. The number of applications you receive has no effect on the match rate, only the number of applicants you choose to rank. 

If the cap is set to low, and all programs feel like they don't have enough applications, we can just increase the cap and notify applicants that is what we're doing. If a few programs don't have enough applications, we can create a new application pool for those programs and let applicants apply to those programs. Finally, if an individual program director is nervous and wants to pull out, they can simply notify every medical school dean in the country that is what they're doing and that they want applicants to apply to their program. 

## This is Simple 

 I make all of this seem really simple. The reason is because this is all really simple. You really shouldn't be having hour long conferences at CORD to talk about how to improve the residency match. I mean you should right now, but in a world with application caps, you really shouldn't. Sure there's a million ways we could make the process of applying to residency more fair, and less painful. But the benefits of those changes would be microscopic compared to just having application caps. 

Sane number of applications? Done. Can easily tell an applicant is interested in your program? They had a limited number of applications, and they chose to apply to your program. Make the process more fair to people who don't already have a bank account balance resembling that of an orthopaedic surgeon? You bet your ass it does. 

Application caps are controversial among applicants, and you'll never convince them that application caps are for their benefit. They are, but you'll never convince them of that. Here's the thing, it doesn't matter. They don't have a say. It is a simple fact that there are far less orthopaedic surgery programs than orthopaedic surgery applicants. Right now, the best way to get into an orthopaedic surgery program is to send an application to every orthopaedic surgery program in the country for the low, low cost of overdrafting your bank account. If you're going to charge applicants more money to apply to more programs, I don't think it should work like that. Medical students have to pay money to screw up an interview at Hopkins, yet I get to do it for free? Program directors, please explain. 

The goal of this service is to make the orthopaedic surgery match what its supposed to be. If you've put the work in to develop a competitive orthopaedic surgery application, you have a handful of programs that you really want to get into, you should have a very high chance of getting interviews at those programs and matching at those programs. If you're a less competitive applicant, not matching is a possibility for you. If you apply intelligently, you could still not match into an orthopaedic surgery program. That's despite application caps, not because of them. At the very least, you could use the money you're saving to apply to another specialty if you weren't already applying to multiple specialties, or a nice new laptop to cheer yourself up. 

This system is really designed to work for everyone. Medical school is structured so that if you get a job application for a residency slot as a program director, you can confidently say that person is qualified to do the work of a medical resident. Medical school slots are relatively limited to the number of available residency slots. The match is supposed to be easy for medical students and residency programs, it just isn't for some reason. The residency match is costly, and complicated because programs have been okay with it being a costly, complicated headache. Most of the problems with the match really do boil down to applicants being able to send an unlimited number of applications. So a service that limits the number of applications students can send, fixes all of those issues. 

## Get In Losers

As I've said, I'm offering to develop and administrate this for free, as long as you pitch in for server costs. I don't want to charge for this, because to quote a recently deceased poet: "it ain't even about the dough, it's about gettin' down for what you stand for yo. For real.". That's what open source is about, a bunch of people have the same problem. So somebody develops an application to solve that problem, takes ownership of it, everyone else contributes to it, and helps make it a success. Then the problem is solved. 

Program directors, what has the AAMC done to address your top 3 pain points from that survey they sent you in 2016 in a substantial way? From where I'm sitting, it doesn't seem like they've done anything. From the outside, it really seems like the match sucks every bit as much as it did in 2016 if not more. If the solution to addressing those issues would reduce the amount of applications med students are sending, that would cost them lost of money. They have no interest in doing it, and they're probably not going to do it. 

ERAS, AMCAS, and the MCAT aren't supposed to be fundraisers for the AAMC. If you're going to hand the AAMC an unfathomably large amount of money for what they're giving you, you should expect they're going to make whatever changes are necessary to make those services the best they can be. If they're not going to do that, you shouldn't have a lot of patience for it. In this case, their loss is your gain. 

The match is something you're going to have to put up with every year until you decide to either retire or you want to own a boat and move to private practice. Why put up with shitty service? None of your problems with the current state of the match are unreasonable. They're also easily fixable. These problems aren't going to go away on their own, and I wouldn't count on the AAMC to go about fixing them. But when the solution is this easy, and the cost is this low: you really gonna say "thanks, but no thanks?".

The match isn't in a good spot. Program directors have the power to make the kind of changes to the match that they want to see, for better or for worse. I've run the numbers, application caps are the only realistic, fair way forward. Just because the AAMC won't implement them doesn't mean you can't have them if you want them. You have the power to make application caps happen. All you need do, is wish it. 
