#!title=Software Lego Pieces
#!path=writings/$
#!use-template=writing
#!order=230
#!audit=JUL2015

If you ever get to look at how I build software, then you will see that I'be achieved building very highly refined component based designs. I remember being a kid writing C++ and being in awe at how generic and useful the Standard Template Library was. I wanted to make generic things that were highly reusable.

It turns out that is hard. However, if you practice and work at it, then you will make useful components that have a shelf-life beyond a single product. I have insight into the secret along with some tips.

# The Secret

The secret is is simply to make lots of things.

If you simply think that you can make a generic thing that does something non-trivial with one to three files, then try to build it in isolation. I prefer to not think when I do this, and just write code as fast as I can. Once I have code, I can play with it and see what I have. I know there is the standard mantra of "Think, Design, then Build". However, I feel this is nonsense.

It is nonsense because this is not how people learn to craft. I'll pull an example from wood working. If you want to make a dove tail joint, then you will realize it is fairly hard. Do you make your first attempts with a $30 piece of exotic hardwood? Or, do you try on a cheap trash piece of scrap wood that is is typically pine? The answer, in this model, is obvious. Use the cheap pine scrap!

The example applies to software in that there is no cost to writing code beyond time. Terrible code tends to cost more time in the long term, so I encourage people to go off and write terrible code in isolation for ideas. This simple ideas tend to build components OR get thrown away. Either result will increase the persons skill someway OR be a success that produces a nice short component. My experience is that the process of writing in isolation before trying to write the real things tends to shave time off building the real thing.

# Tips
## Boundaries
The hardest thing about making generic things is the contractual boundaries of the thing you are building. Again, build lots of things. Patterns will emerge and boundaries will evolve.

## Write lots of code
The theme above is that writing lots of code before design work. You learn about the boundaries of the problems you make, and this will direct the design. You may produce some good components which will improve the design as well, and save time in the building.

## Develop a taste
Use software that works well and has good boundaries. Dig into the code to see how components are built and what patterns emerge. Develop a taste as to what is good. This taste will serve as a mechanism to evaluate the bulk of the code you write.

## Functional
This is why I tend to prefer functional programming ideas since it encourages making generic things via closures. However, you can achieve the same results by practicing in whatever language. I think Java can be a very good language if you learn how to make good lego pieces, but it tends to get abused in terrible ways (which is why Java sucks). Pick a language that encourages good boundaries, and study it. This study will bleed over into other aspects of your craft.

