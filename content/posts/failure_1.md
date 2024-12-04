---
title: 'To learn, is to have failed.'
date: 2024-12-04T22:40:06+05:30
draft: false
tags: ["academics", "research", "theories", "learning"]
---

{{<img src="/posts/science.jpg" alt="Science" class="center" width="50%" height="50%">}}

I think one very important thing that's not talked about frequently is that the best way to learn is to have failed, multiple times.

![fail](https://pbs.twimg.com/media/Ede0UIyWoAIyKmH.jpg)

The above image is one of the coolest depictions of the concept I am talking about but basically the gist is:

{.poetry}
> In order to learn anything, you must first experiment and try to answer the question for yourself, and you will fail, with which you can learn, re-adjust and try again, and again and again. Until you get it right.

This is such an underrated part of the learning process, whether it's learning a new concept or taking the wrong decision for your business. You will, **9 times out of 10** NEVER encounter a situation with all the below parameters:
- The same constraints
- The same circumstance
- The same end result

In System Design this concept is very well illustrated with the **[CAP Theorem](https://en.wikipedia.org/wiki/CAP_theorem)**
![CAP](https://upload.wikimedia.org/wikipedia/commons/c/c6/CAP_Theorem_Venn_Diagram.png)

The ultimate distillation of this particular system design concept is that:
{.poetry}
> Any distributed data system will only guarantee two out of the three requried paramters required for an ideally performant system of the three.

> - **Consistency**: Every lookup recieves the most updated information.
> - **Availability**: Every request must be given a response.
> - **Partition Tolerance**: During any contingency, the system must continue to work despite failures, and can either sacrifice Consistency or Availability to achieve this. 

Not that this has anything to do with Learning and Failure, but the ultimate distillation is that there are no scenarios where you encounter problems with the exact three paramters I described earlier, **unless it's a solved problem.**

Even in the situation that it's a solved problem, you're gonna have to try to solve it for yourself, then lookup the solution and try again. You're not going to learn anything if you haven't failed in solving it already, and this is very critical because this distinguishes scholars from blue-collared work.

No offense to blue-collared jobs, they're pretty cool actually, I find the art of woodworking really pleasant, and electricians are really fucking smart, smarter than electrical engineers due to their unholy intuition of electrical distribution systems.

But I mean the really really low level jobs, like factory line workers jobs, again, I have to be careful with my words, there is dignity of labour in this as well, let's not forget most of consumer electronics from China is done through this very particular facet of the industry, but the truth is they're mindlessly executing a very particular sequence of steps to assemble something at a very fast pace. You get me? This isn't learning at all, it's just, well let's face it, **rote memorization**.

Sure, they're exposed to the internals of the electronic device, but take this person, who's assembling say, a phone and a technician, who do you think can diagnose errors better?
 
You might argue that this is an unfair example, and well it is, but let's closely examine how the entire diagnosis of these errors take place:

1. First, you must identify the issue.
2. List down possible causes, say the screen stops working.
3. Then, you must zero down on the possible avenues within the phone's internals that can cause this.
4. So in this case, it could be - Broken LCD, broken connector pin, fried motherboard, fried ICs, Touch Panel is broken, Fried ribbon cable connecting the screen to the motherboard.
5. Then, a technician must individually supply voltage across each of the mentioned ICs, see if current passes through, if it doesn't, either the ICs are broken, or it could be even worse like blown off resistors / capacitors.

Alright then, cool, what am I trying to say?

Well, technically speaking, the factory line assembly worker kinda has a closer look, and perhaps more time invested in assembling this phone than the technician, but there are some commonalities between these two:

- Both are exposed to the phone's internals.
- Both have experienced in assembly / disassembly of the phone.
- Both have probably even seen that the phone doesn't work after assembly tbh.

Yet the technician clearly knows how to completely solve the phone's problems, and **this is the root of what I am trying to illustrate with my example**.

- The same constraints - Phone screen isn't working
- The same circumstance - Exposure to phone internal components, assembly and disassembly.
- The same end result - Fix the phone screen

Here, the technician has a very crucial **4th factor** helping him achieve this end result:

{.poetry}
> **Failure.**

He has tried to solve this problem before, failed, learned from his mistakes, probably failed a dozen more times, sometimes making the same mistake itself dozens of times, but he has learned. And this, this form of learning, is **incredibly difficult** to **distill**, **compact** and **deliver** to everybody. 

Learning is *inherently* a process of _self-discovery_.

![self-discovery](https://i.pinimg.com/736x/5d/96/c3/5d96c3030166d5507d0db1ce4e676f8c.jpg)

Therefore, truth be told, you can be given direction, you can be pre-informed to avoid certain mistakes, certain adversarial circumstances, pre-instilled with avoiding ambiguity, but you won't know the absolute truths until you walk the path yourself. This is true for **EVERYTHING**.

There's no perfect course for Data Structures & Algorithms, no perfect way to do leetcode, no perfect way to diagnose a patient, no perfect way to achieve enlightenment, no perfect way to solve the hardest problems in physics, no perfect way to avoid getting in fights, no perfect way to do anything in life.

I mean it, you HAVE to make mistakes in life, you have to **Fail Fast, Fail Safe, Pivot and Iterate.**

A really good way of learning, which I guess lies in the [foundation of science](https://en.wikipedia.org/wiki/First_principle#):
![Scientific Method](https://upload.wikimedia.org/wikipedia/commons/thumb/8/82/The_Scientific_Method.svg/330px-The_Scientific_Method.svg.png)
