---
title: Same answer to two questions, or are they?
layout: post
description: Questions matter
tags: math probability
---

You are jogging in the park when a lady, Mrs Smith, walks to you with two babies in double stroller.

- "How cute! Are they twins?" You ask. 
- "Yes they are, but fraternal twins". Mrs Smith answers with a smile.
- "Are they both boy?"
- "No, one of them is a girl".

What's the probability that two babies are both girl?

------

Let's rewind the conversation and change the last question a bit.

- "~~Are they both boy?~~ Can you tell me the gender of one baby and let me guess the other?"
- "~~No, one of them is a girl~~ Sure, one of them is a girl.".

Again, what's the probability that two babies are both girl?

-----
What are the answers to these two questions? Do they have to be same? 

*As I stated in [the last post](https://jiamin.io/2019/09/counting-vs-probability/), when we roll a die, <u>getting 1</u> and <u>not getting 1</u> cover all the scenarios, but clearly they are not equally likely. Therefore listing all the scenarios does not help calculating probability.*

# PAUSE
# THINK BEFORE SCROLLING DOWN
# .
# .
# .
# .
# .
# .

It's probably easy to guess from the title that the answers are different. But why? In both scenarios, we know that **one of them is a girl**. Don't we know the same information in two scenarios? Why would the probability of seeing two girls be different in two scenarios? 

If we want to list all the scenarios - <u>two girls</u> or <u>one girl one boy</u> is one way to do so. But just like <u>getting 1</u> and <u>not getting 1</u>, they probably are not equally likely. We need to list all the scenarios that are equally likely. 

For the first question, it's suffice to list out four cases with same likelihood. Note that we can use an arbitrary feature to distinguish two babies. For example, age/position-in-trolley/name/weight would all work. We use position-in-trolley in the following.

| Left baby  | Right baby | 
|:---:|:---:|
| boy  | boy |
| boy  | girl |
| girl  | boy |
| girl  | girl  |

Note that here we have a hidden assumption that the gender of fraternal twins are two independent and identical events, namely each baby is equally likely to be boy or girl. Our probability bases on this reasonable assumption. 

The answer from the lady rules out the first case.  We don't anything more about the remaining cases -- they are still equally likely. Therefore both are girls, corresponding to the last case has probability 1/3. 

For the second question, the lady is asked to chose one of the babies and reveal the gender of that baby. If we take this choice into consideration, then there are eight cases with same likelihood.
 
| Left baby  | Right baby | Choice of Lady|
|:---:|:---:|:---:|
| boy  | boy | Left|
| boy  | boy | Right|
| boy  | girl | Left|
| boy  | girl | Right |
| girl  | boy | Left|
| girl  | boy | Right |
| girl  | girl  | Left|
| girl  | girl  | Right |

Again it's important to list out all the hidden assumptions because our probability bases on these assumptions. In addition to the assumption above, we also need to assume that the lady will choice with equal likelihood one the children to reveal the gender.

Now we analysis the ladies answer and check the remaining cases. In case 1,2,3 and 6, the lady would say "one of them is a boy". Therefore these four cases are ruled out.  We don't anything more about the remaining cases -- they are still equally likely. Therefore both babies are girls, corresponding to cases 7 and 8 among four remaining cases, has probability 1/2. 

So even if the answers are the same. Same answer to different questions actually leads to different information. 
