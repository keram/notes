---
layout: post
title:  "LDN Functionals #5 - Functional Programming {@Facebook}"
date:   2016-02-13 18:00:00 +0000
categories: meetup
---
# [The fifth LDN Functionals meetup hosted at Facebook's offices in London.](http://www.meetup.com/London-Functionals/events/227340657/)

### Program:

 - [Kris Jenkins](http://blog.jenkster.com/) ([@krisajenkins](https://twitter.com/krisajenkins)):
    [What is Functional Programming?](#kris-jenkins--what-is-functional-programming)
 - Cristiano Calcagno ([@ccrisccris](https://twitter.com/ccrisccris)):
    [Functional Programming At Facebook](#cristiano-calcagno-functional-programming-at-facebook)
 - Sebastian Funk ([@SebastianFunk3](https://twitter.com/SebastianFunk3)):
    [Incremental - Self Adjusting Computations for OCaml](#sebastian-funk-incremental---self-adjusting-computations-for-ocaml)


## Kris Jenkins : What is Functional Programming?

![Kris Jenkins on stage](/notes/images/2016-02-09-ldn-functionals-5/DSCF4110.JPG)

The key point of Kris presentation was that functional programming
is not about specific programming concepts and tools
(higher order functions, map, reduce...)
but about removing the side effects from the code.

He presented *side effects* of a function as the hidden arguments
and hidden output of the function and importance of eliminating them.

It is the same description of functional programming as on Wikipedia but in more approachable words.

> In computer science, functional programming is a programming paradigm—a style of building the structure and elements of computer programs—that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data. It is a declarative programming paradigm, which means programming is done with expressions. In functional code, the output value of a function depends only on the arguments that are input to the function, so calling a function f twice with the same value for an argument x will produce the same result f(x) each time.
> -- <cite>[Wikipedia](https://en.wikipedia.org/wiki/Functional_programming)</cite>

Additional reading:

[What Is Functional Programming?](http://blog.jenkster.com/2015/12/what-is-functional-programming.html)

## Cristiano Calcagno: Functional Programming At Facebook

![Cristiano Calcagno on stage](/notes/images/2016-02-09-ldn-functionals-5/DSCF4111.JPG)

Cristiano presented short history of tool called Infer developed by him and
colleagues in a company called Monoidics which was in 2013 acquired by Facebook.

[Infer](http://fbinfer.com/) is code static analysis tool for detecting bugs
and flaws for Java (Android), C and Objective-C written in [OCaml](https://ocaml.org/)

Code analysis needs not to be just accurate but also:

 - Usable and helpful to developer in way to fix his code
 - Fast and integrated into developers workflow without distractions

As it is impossible or hard and inefficient measure accuracy (number of false positives)
in analyser output, they rather in Facebook measure fix rate of the reported issues by developers.
This number they keep on over 80%.

There was mentioned some other tool from MIT which takes a different approach
than Infer to analyse code but as there is not one best tool
and each has his own pros and cons best assurance is to use them all.

## Sebastian Funk: Incremental - Self Adjusting Computations for OCaml

![Sebastian Funk on stage](/notes/images/2016-02-09-ldn-functionals-5/DSCF4113.JPG)

Very technical talk (thumbs up!)
about a library for incremental computations written in OCaml at [Jane Steet](https://www.janestreet.com/);
one of the largest users of OCaml in the world.

He went from a history of the first version of [Incremental](https://github.com/janestreet/incremental) to latest.

The first version had a naive implementation but it was fast and solved the particular problem.
Next few versions were about improving implementation and expand use cases.
This made the library more usable but in same time significantly slower
than the first version, so later versions deal with speed improvements and optimization of the library.


Additional reading:

[Introducing Incremental](https://blogs.janestreet.com/introducing-incremental/)


---


### Date:

2016-02-09 19:00

### Location:

Facebook Office, 10 Brock St, London NW1 3FG

### Met:

[Johnny Chan](https://twitter.com/jAtlas7), [Shane Gryzko](https://twitter.com/sgryzko), (? guy with dark skin and beard in elevator and outside the building)





