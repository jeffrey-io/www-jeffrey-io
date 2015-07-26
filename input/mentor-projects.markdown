#!title=Mentor Projects
#!path=contact/mentoring
#!use-template=callout
#!order=1
#!audit=STARTED

<font color="red">Note: this page is highly draft, and is subject to constant change.</font>

## Objective

My opinion on the best way to learn how to make software is by making software. This is done by picking up a project and trying to make progress. The purpose then of the teacher/mentor is to be able to help the student/mentee ask the right questions, make progress, and understand core concepts.

### Mentor Project Board (Medium Scope) (HTML/JavaScript/Server)

*Problem:* Managing this list

Design a simple website where people (mentors) can post ideas (like this page), and then mentees can post comments. The requires a very basic understanding the web and either a database or S3. The schema (data layout) is fairly simple. 

### Geo Map Game (WWW) (HTML/JavaScript)

*Problem:* I use uberX in Seattle, and the drivers rely too heavily on GPS. This is problem because GPS is not reliable.

Utilize google maps to provide a game where you ask people questions like "Where is fremont?" or "Where is the Space Needle?", and the people have a clock to find and click the map. Some scoring mechanism will grade the result. This can be done entirely in a single page with a limit number of questions.

### Word Hacking (Terminal) (Anything)

*Problem:* I like winning at bananagrams, but what words are the most effective to know.

The inputs are 
* a dictionary file
* the frequency of letters

The output is a list of words that make me better.

This is fairly wide open problem. How I would start is to experiment with finding the smallest words that are most probable given 21 random tiles. Take these words and then build more complicated words via edit distance. For instace, consider "FEE". I can turn this into "FEET" with a new letter. This can be changed into "FEAT" with another letter.

### Volunteer Machine Organizer (WWW) (HTML/JavaScript and a Server)

*Problem:* There is trash on the highway and streets. What would be great is to help organize volunteers in a more structured way around a map. 

I'm not sure, but it would be nice if people picking up trash and putting them in bags along the road could be organized with people picking up trash bags.

### Markdown Essay Hacker (Terminal) (Anything)

*Problem:* I'm a writer, and my language sometimes lacks.

I would like a very minimal implementation of markdown meant for essays (with little markup). This minimal implementation would expost a list of paragraphs. I would then like to do convert this list of paragraphs into a ".CSV" file (i.e. an excel spreadsheet).

With this in a ".CSV", I would like to upload to Amazon Mechanical Turk to ask random people questions to proof read it.

This can then be extend to take two paragraphs and ask "Does the prior paragraph lead appropriately into the second paragraph?"

Essentially, make it easy to take a 10 paragraph essay and ask 50 people their opinion and speed about $5.

### RAW

* cookie/bakery alert
* web ui to wake
* restaurant menu editor
* universal board game engine
* universal board game server / coordination server
* cookie/bakery alert button
* electronic monitoring for dryer vents
* 3d map generator for world bootstrap
