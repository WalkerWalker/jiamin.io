---
title: Counting vs Probability
layout: post
description: what are the odds?
tags: math probability
---


Welcome to Casino J. There are four cards on the table facing downwards --- <span style="color:red">♥A</span> <span style="color:red">♦A</span> ♠A ♣A. You choose two of them and flip them over. If they are both red or both black, you win. Otherwise, dealer wins. 

Clearly the result can be 

- both red, 
- both black or 
- one of each. 

You win 2 out of 3 scenarios, so you win two third of the time. You bet 10 dollars. If you win, you win 5 dollars. Otherwise, dealer takes the bet. It's clearly a fair game. To express the gratitude for visiting Casino J, dealer gives you 1 extra dollar after each round of the game, regardless of the result. The more you play, the more you win. 

You thought it was totally reasonable and played several rounds with a few wins and loses, until your friend shouted out:"This is a scam!". He then explained, instead of 3 scenarios, there are actually four.

- both red,
- both black,
- first red, second black or
- first black, second red. 

You win 2 out of 4 scenarios, so you win half of the time. The dealer heard your complaints and relunctuntly agreed to change the game slightly as a special bonus. You bet 10 dollars. If you win, you win 10 dollars. Otherwise, dealer takes the bet. 1 extra dollar after each round still applies. 

You felt that you have finally beat the casino, played a few more rounds and left the table with some profit. What a day! You came back home and shared the story to everyone. Your friend laughed to death, saying you were still tricked by the casino. 

So what are the real odds?

#PAUSE
#THINK BEFORE SCROLLING DOWN
#.
#.
#.
#.
#.
#.


Let's list all the result one by one. Note here we do not consider the sequence, because win or lose does not depend on the sequence. 

-  <span style="color:red">♥A</span> <span style="color:red">♦A</span>
-  <span style="color:red">♥A</span> ♠A
-  <span style="color:red">♥A</span> ♣A
-  <span style="color:red">♦A</span> ♠A
-  <span style="color:red">♦A</span> ♣A
-  ♠A ♣A

Clearly from the color we see that there are 2 winning scenarios out of 6, so we only win one third of the time. **What gives?** Can one come up with more scenarios? Is this the right way to calculate the odds?

The truth is all three reasonings are logically not sound. 2 out of 3, 4 or 6 scenarios are fractions of the winning scenarios but **winning probability is generally not same as the fraction of the winning scenarious**, which is essentially the assumption of the following three statements.

1. You win 2 out of 3 scenarios, so you win two third of the time.<br>
2. You win 2 out of 4 scenarios, so you win half of the time.<br>
3. There are 2 winning scenario out of 6, so we only win one third of the time.

To illustrate it a bit more clear. Let's give two more examples.

4. Consider a coin. *Getting head* or *not head* are two scenarios. So the probability of *getting head* is 1/2. <br>
5. Consider a dice. *Getting 1* or *not getting 1* are two scenarios. So the probability of *getting 1* is 1/2. 

This is ridiculous. We all know robability of *getting 1* should be 1/6. But it's not so obvious that in the coin example, the logic, being exactly same as in the dice example, is also not sound. Let's explicitly state again the assumption, which is generally not true, of all above five statements.

**Winning probability is same as the fraction of the winning scenarios.**

So the obvious question is when is the assumption true and not true? We need to find under what condition is the assumption correct. Once this question is asked explicitly, the answer is not far. 

**Winning probability is same as the fraction of the winning scenarios, if all scenarios are equally likely.**

Now it's clear that listing all the scenarios is not enough. We also need to make sure all scenarios are equally likely. In fact, when all scenarios  (finite number) are equally likely, we never need to talk about probability. Simply the counting and fraction argument is enough. Probability gives a richer description when events are not uniform or in the infinite case. 

###AVOID PROBABILITY WHEN YOU CAN
![](/public/images/count/count.png)

Do you agree?



