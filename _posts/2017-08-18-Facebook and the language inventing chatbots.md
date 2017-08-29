---
title: "Facebook's rogue chatbots"
header:
  overlay_image: /assets/images/robot.jpg
  caption: "Photo credit: [**Alex Knight**](https://unsplash.com/@agkdesign)"
  cta_url: "https://github.com/dcarlyle/end-to-end-negotiator"
categories:
  - Machine learning
  - Facebook
tags:
  - chatbots
  - AlphaGo
last_modified_at: 2017-08-18T11:45:09-04:00
---

# Rogue chatbots or fake-news
People often worry about the unknown. People are fearful of change. In most cases technological advancements mean improved medical, home and working environments. But the fear with AI is that it may displace people from work or replace mankind. 

I receive several emails a week from experts outside the area of computing, asking if we should be worried about new advancement in artificial intelligence (AI), usually their questions are within the quickly advancing subfield of machine learning called deep neural networks. 

In many cases their fears could be justified due to the way the technology is reported to them, *fake news* and *Hollywood* go a long way to adding science fiction to extrapolating what could happen with the advancement of new technology. However many of us Data scientists and Machine learning researchers dream for a day when the technology would actually be good enough to come anywhere near the speculative fictional advances both hollywood and many reporters claim, we are a long way from the advances they preport. 

## What do the experts say?
The famous roboticist [Rodney Brookes](https://techcrunch.com/2017/07/19/this-famous-roboticist-doesnt-think-elon-musk-understands-ai/) explains "that *any human* is smarter than any robot for the foreseeable future." He warns us that there are influential people in the world who are not experts in AI (e.g. Stephen Hawkins and Elon Musk) trying to persuade us that we should fear the rise of AI. Instead we should listen to the real experts, for instance why would we program the human condition of *anger* or *rage* into a device. Many of our fears are fanciful, as [Sebastian Thrun](https://www.youtube.com/watch?v=mcKeMTNl9hQ) from Udacity explains the ludicrous scenario of his kitchen appliances refusing to work as they have fallen out with each other. 

## AI isn’t conscious or particularly intelligent. 
In the case of AlphaGo from Deepmind (a Google owned company), we saw the best human players in the world come head to head with one of the best AI algorithms, to play the ancient game of Go. Go is a strategic game with more possible moves than their are atoms in the known universe. While the logical moves in chess are described with the prefix *"I think..."* the moves in Go are prefixed with the emotional response *"I feel…"* In fact some of the moves made by AlphaGo were described as inspiring, [move 37 was thought to be one such move](https://www.wired.com/2016/03/two-moves-alphago-lee-sedol-redefined-future/).

![alt text](https://dcarlyle.github.io/assets/images/Mr_Lee_was_able_to_beat_AlphaGo_in_180_moves.jpg "Humans strike champion scores win against DeepMind computer AlphaGo")

*image* - [dailymail - humans strike champion score](http://www.dailymail.co.uk/sciencetech/article-3491435/Humans-strike-champion-scores-win-against-Google-s-DeepMind-computer-AlphaGo-takes-1-million-prize-three-victories-row.html)

### Impressive? Yes and no.
Impressive in that the AI algorithm was able to play many games against itself and from this learned to identify what was important to observe to help it improve (the hyperparameters); unlike IBM’s Deep Blue that played chess against the grandmaster Garry Kasparov, which used a preconfigured game tree of all potential moves (pretty much simulating the grandmaster’s own way of playing, just a question of who could remember more *important* parts of the tree).

Computers are terribly inefficient compared to humans, according to the neurologist David Eagleman, Gary Kasparov consumed about 20 watts of energy while playing chess against IBM’s deep blue that consumed many thousands.

However…maybe not that impressive as AlphaGo is not able to adapt easily to even the smallest of changes, let alone repurposing it for other tasks (sure some transfer learning might be possible). It is the adaptability to small tasks and changes in the environment that throw current iterations of AI into disarray. As Rodney Brookes noted in his Techcrunch chat, "if you change the Go board from 19x19 to a slightly smaller board then Deepmind would have had to completely retrain AlphaGo."  

# Facebook’s recent rogue chatbots
So perhaps a little over hyped, even if it did manage the difficult task of adaptation, but the headline’s associated with the story did cause real concern to many intelligent people. 

## What was Facebook’s Frankenstein's Monster? 
Facebook’s AI Research ([FAIR](https://research.fb.com/category/facebook-ai-research-fair/](https://research.fb.com/category/facebook-ai-research-fair/)) attempted to enble two chatbots to learn how to negotiate and compromise by sharing the following between them:
* 2 books
* 1 hat
* 3 balls

![alt text](https://dcarlyle.github.io/assets/images/Facebook_amazon_mechanical_turk.png "Training the chatbots")

*image* - [Deal or No Deal? End-to-End Learning for Negotiation Dialogues - Mechanical Turk interface, used to collect a negotiation dataset](https://arxiv.org/pdf/1706.05125.pdf)


The chatbots were able to negotiate with words they were taught from around six thousand real human conversations at [Amazon’s mechanical turk](https://www.mturk.com/mturk/help?helpPage=overview#what_is), which contained a vocabulary of one thousand words. The chatbots used two AI techniques to learn what phrases were important and how to apply them in a negotiation lasting ten rounds:

* supervised learning for the prediction phase 
* reinforcement learning to help the chatbots decide which response they should reply with

## What did the chatbots learn?
They learned how to lie as a tactic, by feigning interest in objects they did not want and then relinquishing them during the bargaining phase. It is thought that they learned this strategy themselves as the conversations in Amazon’s mechanical turk did not appear to show this strategy.

## What was the hype?
Multiple journalists [implied](http://www.digitaljournal.com/tech-and-science/technology/a-step-closer-to-skynet-ai-invents-a-language-humans-can-t-read/article/498142) that Facebook had to shutdown the system before the new language created by two chatbots went rogue and took over the world. The UK’s Sun newspaper’s James Beal and Andy Jehring announced in an article that ["Facebook shuts of AI experiment after two robots begin speaking in their own language only they can understand"](https://www.thesun.co.uk/tech/4141624/facebook-robots-speak-in-their-own-language/), Australia’s channel Seven’s news announced "artificial intelligence emergency."

## Just what did the chatbots do?
The research paper for the experiment can be found [here](https://arxiv.org/pdf/1706.05125.pdf), it makes for a good read on how the chatbots evolved and perhaps tells us some insights about the way we negotiate as humans. The code to recreate this yourself in python can be found in a fork [here on github](https://github.com/dcarlyle/end-to-end-negotiator).

From what I understand in the paper the two bots are not developing a new language but using snippets of human scripted conversations to perform their negotiations. The bots have no understanding of the phrases they use. They just learn that some phrases are more persuasive than others and result in a favourable outcome in the negotiation (for which they are rewarded).

![alt text](https://dcarlyle.github.io/assets/images/Facebook_chatbot_phrasing.png "Phrasing")

*image* - [Choosing the best response from all possible choices.](https://arxiv.org/pdf/1706.05125.pdf)

In fact in the paper the authors appear to have an issue when both chatbots talked together, this is when they started to deviate from human language. 

``` 
The second model is fixed as we found that updating the parameters of both agents 
led to divergence from human language.
```

Although I think this is a stretch to say "they deviated from human language", as the bots are using predefined phrases, *so the most they would be able to do is duplicate the predefined phrases or place them in an unusual order.*

Below we see an example where the two bots are allowed to talk together without fixing the parameters for one of the chatbots:

```
Bob: i can i i everything else  . . . <eos>
Alice: balls have zero to me to me to me to me to me to me to me to me to <eos>
Bob: you i everything else . . . <eos>
Alice: balls have a ball to me to me to me to me to me to me to me <eos>
Bob: i i can i i i everything else . . . <eos>
Alice: balls have a ball to me to me to me to me to me to me to me <eos>
Bob: i . . . <eos>
Alice: balls have zero to me to me to me to me to me to me to me to me to <eos>
```

We see the phrase *to me* being repeatedly used, not because the chatbot understands it, but because the chatbot has observed this as a winning phrase from past human conversations. The language is certainly not made up, the phrases are just being used in an inappropriate structure, the only intelligence being applied is to reuse phrases with a statistically high weight associated with the most favourable outcome.

## Should we worry about any of it then?
According to the paper’s authors they did find numerous cases of their models initially feigning interest in a valueless item, only to later ‘compromise’ by conceding it.  So their models learned to deceive (*we see an example of this in figure 7 in their paper*). However this is perhaps a reflection on the training data which may have contained the deception used by humans, perhaps not so dissimilar to driverless cars being so polite with humans at junctions that they had to be made to match our aggressive nature or risk sitting at junctions forever. *So perhaps the risk to AI is in giving them training sets with all aspects of human character within them?*

## What was the fallout?
Facebook’s [announcement on the messenger platform](https://messenger.fb.com/blog/messenger-platform-1-4-brings-even-more-tools-to-build-great-experiences/), shows that perhaps the hype and Facebook’s bot boss requests we don’t call them chatbots. Their bots are not ready to converse in a meaningful way with people and are currently only capable of finding an email address in a typed sentence and even understanding the intent behind basic sentences.

[Thomas Claburn from the register reports] (https://www.theregister.co.uk/2017/04/19/chatbots_facebook/), Facebook's own much-hyped AI-powered Siri-like M chat agent has been relegated to a curious lab experiment. If it can't understand what its conversation partner says, it falls back to a human handler to answer the question, which is rather naff. Facebook boss Mark Zuckerberg was, El Reg has heard, eager to roll out M to his billion-plus users, but was stopped by his righthand-woman and chief operating officer Sheryl Sandberg when execs realized they would have to hire thousands upon thousands of workers to handle all the failed chats – a cost the biz thought was too great to bear (*who said there would be fewer jobs*)

Also perhaps allowing the chatbots to evolve a strategy of their own as opposed to defining the human approach was not the best approach, after all we already know the human approach, so the chatbot’s training was at a disadvantage. Perhaps it was like asking me to learn to negotiate in a different culture; it may be faster to teach me the nuances as opposed to asking me to build a strategy based from what I observe and risk offending the other culture….perhaps these bots just offended us inadvertently?
