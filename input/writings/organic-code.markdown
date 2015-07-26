#!title=Organic Code
#!path=writings/$
#!use-template=writing
#!order=2
#!audit=JUL2015

Software peoples (Hackers, Coders, Programmers, Developers, Software Engineers, etc...) as a group (mostly) want to make good code. The core problem is that code quality does not exist on a spectrum from bad to good. It is very easy to armchair arbitrate code quality and say "oh, that code is bad because {X}" rather than focus on what the code does well. I know I'm guilty of this.

The core reason we care is because we the software peoples have to deal with code every single day, and we like making our customers happy. Bad code makes us unhappy as it becomes difficult to extend and support. The paradox that I have seen is one can make a product with good code, but all it takes is one feature request to induce a realization why it is all wrong and bad.

Code quality is a multidimensional beast, and it is very hard to measure. Does this mean we should give up and just do what we want? Well, I think defining good code leads to a path of painting a bike shed because personal taste can dominate what good code means. Instead, I want change the game. Instead of thinking about code as good and bad, I want to create some conditions for "Organic Code".

"Organic Code" is code that could be bad, but it has the hope to become good by whoever is maintaining it without a massive rewrite. So, without much more introduction, I shall now iterate the criteria for what makes code organic.

### Work as Advertised

If your code advertises as doing something, then it better do it. This, in my opinion, is the most minimum bar for shipping anything. I really do not like it when people pee on my leg and tell me it is raining, and I appreciate the same with software. 

### 100% Unit Test Coverage

Unit test coverage is not magical. It means I have mocks for my external dependencies which I can use to simulate various failures, I verify that I at least touch every line of code, and I touch all branches at least once. My personal perspective is that getting 100% unit test coverage is a very low bar. I do not believe in code that can not be tested anymore, everything is testable. If the cost is deemed to high to test, then something is very wrong.

You may think unit testing isn't needed for your project, and you may be right; you just have to accept it will not meet the "Organic Code" stamp of approval. The benefits of 100% unit test coverage is this:

* Ability (Or, at least, hope) to add tests to prevent regressions of bad behaviors
* Provide a level of safety for the next guy to refactor
* Provide confidence the code at least does something right

Honestly, I can see people argue about the percentage of code coverage, but anything less than 100% is not organic. It has been my experience that code which is not easy to test is not well designed. If you focus your code writing with the emphasis on "I am going to test this", then it becomes a new game.

#### External Dependencies

When you mock an underlying layer, there is always the actual layer code which requires testing. This code, needs to achieve 100% coverage as well via integration testing. Ideally, you will have integration environments for separate test environments from prod.

### Enforce Contracts

When I break a known contract (i.e. a function name or signature), then my tool chain and tests must prevent me from shipping. I need to know that I broke bad. There are ways of doing this in every programming language, but it is easier in statically typed languages. Keep in mind, statically typed languages do not mean you can not make stupid contracts. Organic code, by this nature, must not have overly stupid contracts. Some rules to avoiding stupid contracts:

* Do not overload method/constructor names (Highlander rule := there can be only one)
* Have descriptive names/variables with rich types 

For instance, if your language supports enumeration and Boolean types, then prefer enumerations. It is way better to have an enumeration with two values that are descriptive rather than having Boolean types. This means that method signatures will make sense later rather than having a sequence of Boolean, Boolean, Boolean, Boolean...

### Avoids Over Engineering

The more experienced of engineer one becomes, the more patterns and practices one is aware of what makes software "good". Patterns are great, but they can become a burden in the future. Organic Code should start as simple as possible without too many layers. This induces future costs for when aspects need to be generalized. Personally, I would rather generalize simple code rather than deal with code that has a bunch of patterns that yield little value.

The first code to be checked in for an organic code base are like seeds: very simple and tiny. They express the primary goal of the project. It may not address the scale needs, nor will it have all the extensible features. It will be the most simple pattern imaginable at the time. This, of course, is subjective. However, it is easy to see over engineering:

* Are there interfaces used only once which have no clear future
* Does it have events which serve little purpose to achieving the goals of the project?

Ideally, organic code's first check in serves as inspiration for what the thing should be doing.
