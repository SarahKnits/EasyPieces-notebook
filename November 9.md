#Design notebook for week ending November 9, 2014

## Description

I've spent time this week fleshing out what my preliminary input syntax will
be, along with testing out the output. At present, I will be copying the output
into Mac's Grapher application, but I am working on figuring out a better and
cleaner solution. 

I have written a basic parser for a single function that extracts the function
name, variable, condition, and equation. I will soon be adding some basic
error checking, such as verifying that only the given variable is used in the
equation, simplifying equations when possible, and catching illegal operations
such as division by 0.

For a clearer idea of my preliminary grammar, check out sampleInputs.txt in the
project directory. 

**Checking in with my goals**

Week 2: I will have the IR for my MVP defined and a basic input (even if it is not the final one I use). I will also have a first idea for the output.

By this week, I expected to have the IR defined along with a basic input.
Both of these have been defined and can be found in my project files.
I am questioning whether Grapher for Mac is the best option, but I am
basing my preliminary design on the idea that the output will be for 
Grapher.

## Questions

**What is the most pressing issue for your project? What design decision do
you need to make, what implementation issue are you trying to solve, or how
are you evaluating your design and implementation?**

The most pressing thing right now is figuring out which graphing program to
use. I would really prefer to use Grapher for Mac, but it doesn't look like
I'll be able to format the input in the way I want. I'm also considering 
gnuplot.

### Pros and Cons of Different Graphing Tools
#### gnuplot
##### Pros 
* Complete flexibility - I can make the graph look however I want

##### Cons
* More complicated output
* More needs to be defined by the user or calculated using logic

#### Grapher for Mac
##### Pros
* Very easy to graph - Just copy the text in

##### Cons
* Less flexible
* Requires more effort from the user


**What questions do you have for your critique partners? How can they best help
you?**

I would appreciate feedback on my preliminary grammar as well as any
suggestions for which program I should use for the final graphs.

**How much time did you spend on the project this week? If you're working in a
team, how did you share the labor?**

I spent 3 hours defining my preliminary grammar and coding out the parser for
it, 2 hours researching possible programs to use for the final output, 1 hour 
working on the notebook and documentation, and 1 hour completing the critique 
for my partner. 
 
## Post-critique summary

Alex emphasized the importance of finding a good graphing software to cut down
on the amount of coding I have to do. He also suggested that I stick with the
piecewise functions and simple 2D functions initially and then expand after
that if there is still time. He also suggested variables to hold reusable
code fragments.

## Post-critique reflection

I like the idea of using variables to store reusable code fragments to prevent
the user having to retype a piece over and over.

I know that the graphing API will be the most important decision to make, as it
will define what will be possible and easy to implement in my language. I also
recognize that the design decisions are otherwise somewhat limited, and that I
may need to expand my scope to include more creativity and designing.


