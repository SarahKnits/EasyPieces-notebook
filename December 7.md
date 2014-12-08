# Design notebook for week ending December 7, 2014

## Description

This week was a lot of polishing and trying to finish up my project. I added
meaningful error messages that helped my test users figure out what was wrong
with sample broken programs. I also fixed the tests. I had started out my 
development process by writing tests, then failed to update them after that
point. I now have useful tests that can make sure future changes don't break
existing programs. The tests don't check the actual graph output, but make sure
that the mapping is correct. I have also manually checked many graphs. 

This week I also spent time figuring out what the ideal step size should be. 
GNUplot has issues with graphs where too many points are too close together. 
Although I didn't follow the entire idea Alex proposed (calculating the change
for each point and making sure the change is never greater than some epsilon),
I found a balance between having major aliasing issues and having some lines 
not show up. 

## Questions

**What is the most pressing issue for your project? What design decision do
you need to make, what implementation issue are you trying to solve, or how
are you evaluating your design and implementation?**

At this point, I don't have many design decisions that need to be completed
before I turn in this project. The following are some design decisions that 
would need to be made to add to the project:

* What should the user interface look like?
    - Eventually, I'd like to have a GUI to input and show the graphs
* More thorough stepsize calculator
* Graphs over the entire domain
* More fine control of graph output without overwhelming novice users
* Correctness checking for limits

**What questions do you have for your critique partners? How can they best help
you?**

Do you have any (relatively small) suggestions to improve the quality or 
usability of the program? Anything that should change in the error messages?

**How much time did you spend on the project this week? If you're working in a
team, how did you share the labor?**

This week, I spent about 2 hours working on error messages, 1 hour on user
testing and evaluation of those results, 1 hour working on testing, and 30 
minutes writing up the notebook. I also spent 1 hour reading my critique 
partner's project and documentation and writing my critique. 

## Post-critique summary

Alex said that my project looks mostly good so far (yay!), and that I should
focus on making meaningful error messages. He also mentioned that the open curly
brace made him unhappy, but said that it was alright if my non-CS testers were
okay with it. 

## Post-critique reflection

 I spent a fair bit of time this week making my error messages meaningful and
 testing them on non-CS users. I'm going to keep the curly brace.
