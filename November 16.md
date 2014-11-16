# Design notebook for week ending November 16, 2014

## Description

One thing I need to get done this week is defining the order of operations for
the bounds and functions. I plan to conform to PEMDAS rather than just 
left-associativity, but I will have to figure out how possible that is. 

I will make sure I have properly accomplished this task by writing tests that
check that the right associativity is being used. 

I am also trying to figure out whether I will need to simplify the bounds and
functions or whether I will be able to leave the final calculations up to the
grapher (if I use an existing grapher). 

I spent a fair amount of time this week researching different graphing libraries
to determine which one I ought to use. I found that Scalaplot allows me (or the
user) to graph piecewise functions and output in various forms, such as png, 
ASCII art, and PDF, as well as having the option to launch a plot viewer that
allows the user to resize the graph and save it. 

I found that the Grapher file format (gcx) is binary and not possible to easily
replicate. Scalala/Breeze has some nice functionality, but a lot of overhead
that isn't needed for this project. 

As of now, I will be moving forward with Scalaplot. 


## Questions

**What is the most pressing issue for your project? What design decision do
you need to make, what implementation issue are you trying to solve, or how
are you evaluating your design and implementation?**

The most pressing issue this week was what graphing tool I would use for the
output. I think that Scalaplot's output is very close to my ideal, and I have
now figured out what the code for that output will look like. My next step
will just be using my AST to generate code for the output. 

**What questions do you have for your critique partners? How can they best help
you?**

I would appreciate if you could try running the program for yourself without
downloading any of the graphing tools. I want to make sure that everything is
properly included in the build.sbt file.

Also, does the sample graph output (see below) look like you would want the 
piecewise graph to look? What else might you want to add?

![Program 2 Graph](https://github.com/SarahKnits/project/blob/November16/piecewiseGrapher/docs/img/SecondProgram.png)

How highly should I prioritize allowing different variable inputs than "x"? As
of now, I am considering returning an error if the variable is not "x", but I
am wondering how often it would be useful to have a different variable. 

For now, I am using a step-size of 0.01. How much should I prioritize figuring
out the ideal step-size instead of just sticking with 0.01?

**How much time did you spend on the project this week? If you're working in a
team, how did you share the labor?**

I spent two hours working on the input, two hours researching different graphing
tools to use, two hours figuring out what the code for the graphing output
would need to look like, two hours thinking about and considering the design and
implementation file, 

## Post-critique summary

Alex commented that he would have preferred the function specification to be
more explicit rather than using otherwise. 
Alex also suggested two possible paths for the project moving forward: expanding
the language to handle more complicated functions or making the user interface
as fabulous as possible. 
The last recommendation was to use Grapher instead of GNUPlot. 

## Post-critique reflection
For the explicit function specification, my decision to use otherwise was
trying to best match the format of given assignments, so I will stick with my 
original decision on that part. 

For future development, I will spend most of my time expanding the language to 
handle more complicated functions (probably still 2D for now) with at least a 
little bit of time spent on optimizing the user input. I hope to be able to 
handle the vast majority of functions anyone would need to graph properly. 

After my research and reflection this week, I don't think it will be possible to
use Grapher. What I meant by having difficulty formatting the input is that I
would output a text file that the user would then have to manually copy line by
line into Grapher which seems a suboptimal user experience. ScalaPlot, the
program I have decided to use for graphing, is a Scala interface for GNUPlot.

