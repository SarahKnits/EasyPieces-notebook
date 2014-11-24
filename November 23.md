# Design notebook for week ending November 23, 2014

## Description

### Language Extension

This week, I wrote the majority of my Semantics. At this point in the project,
it is possible to graph simple polynomial functions, sine, cosine, absolute
value, e^x, and square root. Most things I want to implement work properly
as long as the input is correct. 

### Error Checking

Right now, error checking is lacking. One of my next steps will be to provide
helpful error messages if parsing fails or if the input is invalid. I plan to
add correctness checking in the following areas:

* Overlapping bounds - each function only covers each x value once
* Defined at all points - no division by 0 or other undefined behavior
* Proper bounds - no bounds a < x < b such that b <= a
* Correct variable used

Other possible error checking:
* No x values without a y value

## Questions

**What is the most pressing issue for your project? What design decision do
you need to make, what implementation issue are you trying to solve, or how
are you evaluating your design and implementation?**

At this point, I have finished most of my goals for the project. The ongoing
issues are as follows:
* Improving input
* Error checking
* Better error messages
* Other functions
* Order of operations
* Doubles instead of just integers

I plan to prioritize error checking and error messages for this coming week. I
will then work on improving the input and adding additional functions that may
be useful. 

**What questions do you have for your critique partners? How can they best help
you?**

Are you able to run through the tutorial? Did you have to download anything
beyond GNUplot to get it to work? How would you improve the input? 

**How much time did you spend on the project this week? If you're working in a
team, how did you share the labor?**

I spent about an hour figuring out what extensions would make sense for my
language, three hours adding additional functionality, an hour and a half
completing the  project notebook, and two hours writing a comprehensive 
tutorial. I also spent an hour critiquing my partner this week. 

## Post-critique summary

I got feedback that the output looks good, and that it would be a good idea to
have the bounds explicitly specified for the displayed graph. It was also 
recommended that I allow the user to set the labels for the x and y axes. He
also recommended that I add additional functions such as sine and cosine,
parentheses, and proper order of operations. 

He proposed two possible ways to find the proper step size - one dynamically 
calculating the point at which the value of the function doesn't change more
than some epsilon over the step and one simply dividing the total x-values by 
10,000. 

## Post-critique reflection

I will add in an input option for the labels for the x and y axes. I took the
critique into account when I added sine, cosine, and parentheses, and I will 
be adding order of operations in the coming weeks. I think I will probably go
with the second suggestion for the step size (dividing the total range by
10,000) for now, and I may make it more complicated in the future. 


