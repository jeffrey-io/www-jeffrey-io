#!title=Abstraction Power
#!path=writings/$
#!use-template=writing
#!order=199
#!audit=MAY2015

# Brevity

I have been writing code since I was about nine. I started with BASIC on an IBM PC with an 8088 processor. The thing about the time from when I started until my mid twenties was that I wrote a ton of code. The last time I tallied, I was well early millions lines of code. This is why my wall of shame is so shameful because I wrote more code than I needed it. I have noticed that over the years, my ability to write code with brevity has only increased.

> I have only made this letter longer because I have not had the time to make it shorter - Blaise Pascal

Now I find myself in a sticky situation since I work with others (and I am the old guy in the room). This is a sticky question because I want to help them out, but this tends to resort to me telling the answers. Or worse, when people move on, I just do it myself. At some level, I have to come in and help out with answers to make sure we hit deadlines. As I build in my adult capacities, I need to start thinking about more concrete advice to help the youngsters. So, after this next quote, I'll digest my current thoughts on this subject.

> It is my ambition to say in ten sentences what others say in a whole book. - Friedrich Nietzsche

# Advice

## Finish on Time

I tend to view getting things done is better than entering an endless refactoring party. I love to refactor and make sense of the world, but I also like to move towards more interesting projects. If you develop the discipline to (a) ship code and finish, and (b) study your code critically, then your next project will go smoothly.

> Be sincere, Be brief, Be seated. ― Franklin D. Roosevelt

## Replicate Twice, Reduce

There is nothing more infuriated as an abstraction (like a Java interface) that only has exactly one logical implementation. My advice is that when you see a problem, and it starts to resemble something else. Finish it the way you started. Once you have the two solutions, then you have enough data to help simplifying the world. If you do this, then you will find that refactoring will reduce the testing needs. In other words, instead of writing new tests, spend time refactoring your old code to allow for new functionality.

> A novel is just a story that hasn't yet discovered a way to be brief. - George Saunders

## Architecture Kata

I didn't grow up with the idea of [code katas](http://en.wikipedia.org/wiki/Kata_(programming)), but I think it is a useful concept. I recommend taking it a step further and do an entire architecture. I give this advice because I saw a clear progression in one of my bigger projects growing up. Naturally, I started programming to learn how to make games. This meant I needed a game engine. So, I made my first 3D engine in college. It was well over 100K. I didn't like it, so I rewrote it to add a few new features. I reduced the code base to 60K. Again, I didn't like it, so I rewrote it again. This final time, I got all the same features in about 25K.

> Good things, when short, are twice as good. - Baltasar Gracián y Morales

## Learn Math and Functional Programming

I'm surprised how helpful both abstract algebra and functional programming has been to my building of stuff. I highly recommend spending an evening or two dedicated to working in an ML language like OCaml or Haskell. The reason this works is because you almost have to be brief with you code since everything is a pain if you don't know the operators like map, foldl, filter. When you learn these things, they just make sense.

As to algebra, I have found that many functional programming ideas can be expressed with algebraic thinking. I'll leave this discussion for a later date since most people are not prepared to go to that depth.

> Brevity is the soul of wit. - William Shakespeare
