# clean-code

## code smells

### comments
* comments are a manifestation of the the developer's inability to 
manifest intent in the code.
* comments lie.
* comments should be avoided at all costs.
* comments should really be in a readme/documentation/markdown file.
* for the love of god, don't do it. ;)
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