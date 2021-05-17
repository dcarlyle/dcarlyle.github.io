---
title: "Ethical AI"
header:
  overlay_image: /assets/images/robot.jpg
  caption: "Photo credit: [**Alex Knight**](https://unsplash.com/@agkdesign)"
  cta_url: "https://github.com/dcarlyle/end-to-end-negotiator"
categories:
  - Ethical AI
  - Ethics
tags:
  - ethics
  - AI
last_modified_at: 2021-05-11T11:45:09-04:00
---

# Ethical AI quandaries

Whilst pondering the ethical issues around autonomous driving last week and why Toyota had only opted to go for autonomy level 2 (no feet or hands) whereas Telsa was opting for autonomy level 4 (no feet, hands, eyes, brain), it struck me that this was not a question about Data Science but about AI’s Ethical impact in a social environment. This is another very clear distinction between AI and Data Science, where the strategy of a social environment comes into effect. The old conundrum of the _run away trolly_ do we do as Mercedes MD would do and save the occupants of the car or do as the Twitter followers suggest and protect the pedestrians. I think we do what the strategists suggest and remove the cyclists and pedestrians, as we currently do on the motorways, where both cyclists and pedestrian are restricted as we cannot both drive at speed as humans and protect others.

![alt text](https://dcarlyle.github.io/assets/images/hack_boneh.jpg "Prof. Boneh hacks STOP sign image, turning it to a 40 mile an hour image to a driverless car's CNN, just by adding 4 stickers") Another issue to be considered is around the early release of a model before they are fully tested and productionised. Take for example this simple STOP sign image, with four strategically placed stickers to fool a driverless car's image recognition into believing it has observed a **40 mile an hour street sign**. The consequences could be devastating for the car, its occupants and anyone in the car's path as it jumps a STOP sign and accelerates on. This particular example **did not even require code** to hack the neural network, just a few simple stickers to upset the probabilistic model. Is it ethical to release a model into the real world which has the potential to be hacked? 

Ethical AI is a very fascinating area, as there is a balance between computers being helpful or overstepping into what we might consider being “creepy” or a “loss of control.” Computer ethics teaches us a lot about ourselves and our own culture, as buried within many data sets is a history of our cultural beliefs, none better than that from 600 years of case histories from the old bailey, an amazing data set but with an evolution of our culture contained within. For instance, if I use the old bailey data set to train an AI to judge us, it might suggest that using excessive force is acceptable if someone were to steal something as nondescript as your pen.

Not only do data sets encapsulate our culture, but they can also be skewed on where the information has been captured. I know that one of the issues we had with medical data sets was that the bulk of the data was captured from Northern European Males, which meant dosage measures and the analysis of the impact on phenotypes would fall short or other groups of patients. 

## Diversity
Netflix recently released a lovely documentary around bias data sets https://www.netflix.com/gb/title/81328723, following Jo, an AI researcher at MIT and her petition with the USA government on Gender and race bias in data. Jo, discusses the controversy of the AI and in one particular example, the everyday practical implications applied to a soap dispenser's inability to detect her hands.

My career started with looking at the bias in Algorithms as opposed to Data Sets. My focus was on how I could use psychology in my algorithms to gain more time from the customer in order to buy more time to process their data, this was back with dial-up modems. Today we see this in computer games, an industry worth £5.5 billion in the UK alone, which use techniques to slow the player down while they load the next scene. Psychological manipulation of the customer is employed in most User interfaces and more recently in chatbots, to seek empathy and fool us into a sense of security.

A few years back, I was asked to write an article for Mensa, after publishing a blog post to discuss the limitations of AI for a very concerned friend who was the founder of Shazam which sold to Apple last year for $400 million and using a lot of AI in his business, who was worried about the “rise of the robots”  and the world in which his children might inhabit. In that article, I showed that there are some fundamental obstacles to overcome, and also some reasons why his children will remain safe. So relinquishing control to AI is a genuine concern of some of the tech leaders.

The amazing Hannah Fry in her recent book discusses the America company Comapsss who built an algorithm to assess probation periods for ex-offenders. This particular debate was about allowing non-publicly viewable algorithms to make decisions that impact human's lives at a profound level and should we have the right to see the inner workings. However when the algorithm is hidden from us we can often still find how it works and that access is escalated in AI where some computer scientists using a technique known as _Shadow modelling,_ are able to reverse engineer the proprietary algorithm and extract the original sensitive training sets on which the AI was trained. In Hannah's example, she goes on to explain that the algorithm perhaps didn’t measure enough of the important societal factors impacting the ex-offenders, e.g. ability to access child care or a working mode of transport. 

## Our social data
In China, they have a social scoring tool known as _Sesame_, as you disembark the train on the way into Beijing a passenger is reminded that if they have a score over 500 they can apply to travel on a holiday overseas or use a 5-star hotel. This might seem abhorrent to us, but it is something they have visibility of, for us in the West, large tech rather than our governments make those decisions, e.g. my food purchase data is shared with insurance companies and from this, they can determine if I am a model citizen and less likely to call on my household insurance all from observing if I buy _dill._ 

I think writers have an amazing way of looking at the social and ethical impact of new technology and help us to visualise and ponder the impacts. This is a fun explanation of the social scoring dilemma from Charlie Brooker - https://www.youtube.com/watch?v=R32qWdOWrTo

## Too many insights
During my work in Vietnam with the government to analyse accents, we very quickly started to show insights into where a person was educated, if they were a native speaker, all from their voice. This threw up an ethical dilemma for me, in had I crossed a line? There are many such examples today where the gathering of data which could proove to be of benefit could also be seen as intrusive, like the use of smart meter data to detect my use of appliances via their energy consumption signature being linked to the time of day to indicate if I have early onset dimentia, years before I am even aware.

## Industry
Where I can see ethics in the UK becoming increasingly important to Industry are around our advances in driverless cars: 
* Around decisions over allowing a car to override a human, e.g. a child being driven to school and the child suggests an alternative faster route down an empty one-way street, but going the wrong way; who determines the outcome the human, or does the AI overrule the under age occupant.
* Should a car in an unavoidable collision manoeuvre the car to hurt more people, but in a less fatal manner or hit fewer people, but with more fatalities.
