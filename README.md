# clean-code
* The code we write is a manifestation of what's inside our hearts and 
our minds.
* Meditate, clear your heart, and mind before you write any code.
* Every line of production grade code we ship, must have a line of 
production grade automated test that will self validate itself.
* If all the tests pass, we ship. 
* Love is the most powerful force in the universe. 
* When you write your code, make sure it's built, powered and tested 
using pure love.

## clean code characteristics
* code quality = WTFs/minute. less is better.
* "I like my code to be elegant and efficient. 
The logic should be straightforward to make it hard for bugs to hide, 
the dependencies minimal to ease maintenance, error handling complete 
according to an articulated strategy, and performance close to optimal 
so as not to tempt people to make the code messy with unprincipled 
optimizations. Clean code does one thing well." - Bjarne Stroustrup
* "Clean code is simple and direct. Clean code reads like well-written 
prose. Clean code never obscures the designer’s intent but rather is 
full of crisp abstractions and straightforward lines of control." - Grady Booch
* "Clean code can be read, and enhanced by a developer other than its 
original author. It has unit and acceptance tests. It has meaningful 
names. It provides one way rather than many ways for doing one thing. 
It has minimal dependencies, which are explicitly defined, and provides 
a clear and minimal API. Code should be literate since depending on the 
language, not all necessary information can be expressed clearly in code 
alone." - “Big” Dave Thomas
* "I could list all of the qualities that I notice in clean code, but 
there is one overarching quality that leads to all of them. Clean code 
always looks like it was written by someone who cares. There is nothing 
obvious that you can do to make it better. All of those things were 
thought about by the code’s author, and if you try to imagine 
improvements, you’re led back to where you are, sitting in appreciation 
of the code someone left for you—code left by some- one who cares deeply 
about the craft." - Michael Feathers
* "In recent years I begin, and nearly end, with Beck’s rules of simple code. 
In priority order, simple code:
** Runs all the tests;
** Contains no duplication;
** Expresses all the design ideas that are in the system;
** Minimizes the number of entities such as classes, methods, functions, and the like." - Ron Jeffries
* "You know you are working on clean code when each routine you read 
turns out to be pretty much what you expected. You can call it beautiful 
code when the code also makes it look like the language was made for the 
problem." - Ward Cunningham
* "The only way to go fast is to go well." - Robert "Uncle Bob" Martin

## code smells

### comments
* comments are a manifestation of the the developer's inability to 
manifest intent in the code.
* comments lie.
* comments should be avoided at all costs.
* comments should really be in a readme/documentation/markdown file.
* exception: comments are allowed in the commit log or pull request, 
but not in the code.

#### c1. inappropriate information
* metadata such as authors, last modified date, spr number, etc 
should not appear in comments. 
* comments should be reserved for technical notes about the code and design.

#### c2. obsolete comment
* a comment that has gotten old, irrelevant, and incorrect is obsolete.

#### c3. redundant comment
* a comment is redundant if it describes something that adequately describes itself.
* comments should say things that the code cannot say for itself.

#### c4: poorly written comment
* a comment worth writing is worth writing well. 
* think of comments like tweets, find the zen of what you are trying to say, 
and express it well. 

#### c5. commented out code
* delete it immediately, it is forbidden.

### environment

#### e1. build requires more than one step
* You should be able to check out the system with one simple command and 
then issue one other simple command to build it.
* `.love> ./build.sh`

#### e2. tests require more than one step
* you should be able to run all the unit tests with just one command. 
* `.love> ./test.sh`

## references
* martin, robert. clean code. a handbook of agile software craftsmanship.