#!title=Build First, Buy Second
#!path=writings/$
#!use-template=writing
#!order=1

Most projects involve a series of decisions revolving around building your own inhouse or buying an off the shelf product to adapt. For clarity, buying could mean picking up a free open source project. You can already infer my opinion from the title, so I'll justify it now.

Without a doubt, you should always invest time up front to build your own first at least once. The key to not going down the yak shaving spiral is to time box your effort, and just simply try. There is where I have to disagree with Yoda. 

> Do or Do not. There is no try. - Yoda

I believe experimentation is central to learning, and Yoda is a fictional character. That being said, I'll lay out suggestions which I believe builds a better foundation for understanding most buying decisions in the future. If you spend a year on the below curriculum (say, 10 hours a week), then you will be better off both as a builder, a hacker, and an engineer.

# Desktop Curriculum

## Notepad

It is very easy to throw a text control into a window, add a menu bar, then claim to have invented a new text editor. However, how does the text control actually work? It has been my experience that learning to create a control is enriching as you learn

* state machines for mouse behavior
* font metrics
* basic drawing primitives
* various graphic techniques like dirty rectangles, double buffering, and caching bitmaps

The nice thing, once you get the bare bones text control done, then you can have the real fun. Can you add things like folding, syntax coloring, or copy and paste?

## Games

This section is usually redundant as many of us got into this business due to the magic of video games. That's why I am here, and it also how I have done so much. The hard part, for me anyway, of making a game is focusing on the game rather than the game engine. I like making game engines, but a game engine should be a consequence of a game. That being said, making a game involves

* some kind of ui aspect
* various state machines for play mechanic
* enforcing rules
* the classic take input, update state, render loop

### Suggestions

* board game like monopoly, risk
* puzzle game like tetris
* top down 2D rpg

Once you get past the programming, the big reveal is that a typical game is usually 90% art.

## Game Engine

The yak-shaving aspect of making a game is that you focus on making the game engine. For simple games (like the above suggestions), it is very simple to just make them. However, suppose you wish to create a 3D world. Now, the nice thing is: this is a great adventure. The unfortunate thing is: it can be very hard. For this aspect, I highly suggest going through <a href="http://www.amazon.com/gp/product/0122290631/ref=as_li_ss_tl?ie=UTF8&camp=1789&creative=390957&creativeASIN=0122290631&linkCode=as2&tag=zenerdcom-20">3D Game Engine Design: A Practical Approach to Real-Time Computer Graphics (Morgan Kaufmann Series in Interactive 3D Technology)</a><img src="http://ir-na.amazon-adsystem.com/e/ir?t=zenerdcom-20&l=as2&o=1&a=0122290631" width="1" height="1" border="0" alt="" style="border:none !important; margin:0px !important;" />; this book is an amazing guide for learning all the math and design patterns to build a rendering engine. Once you have a rendering engine, you have (most) if all the primitives you need to create a 3D world.

## Custom Controls

Like a notepad, what if you want to make a rich editor for images? What if you want to make your own slider? What if?

### Suggestions

* map editor for 2D games
* image composition (layering)
* gui editor

# Server Curriculum

## Web Server

How does HTTP work? I am a huge fan of sitting down, at least once, and writing a http server from bare sockets. Doing this, you will learn

* sockets and tcp basics
* basics (i.e. 80%) of the http protocol
* concurrency model (single threaded, multithreaded, and maybe asynchronous)
* thoughts about how to generalize (cgi? fast-cgi? servlets?)

&&networking&&

## Web Framework

Take any web server (even your own), it is going to suck to build a product on it. Try to make it suck less. Doing this, you will learn

* about url routing and linking
* asset organization
* templating
* some separation of the data tier to the html production

&&front-end&&

## Database

Simple, model your problem first with flat files. It is surprisingly easy to avoid all the reasons you would need a database and get something working that demonstrates what you want. Once you know what you want, you are in a better position to buy the right package; the beauty is the cost is entirely justifiable because you did the proper research to understand the problem. Take your solution, then slap a web server on it, and now you have an API.

# End Goal

If you follow this advice, then you will be a better hacker, engineer, builder for it. This is not an exact recipe for success, but it paints a picture of what has worked for me and others I have worked with. I think living as a software person requires an active curiosity of how things work and how things are built, and the best way to learn is by doing.
