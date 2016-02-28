---
layout: post
title:  "Functional Programming for the Web"
date:   2016-02-13 18:00:00 +0000
categories: meetup
---

### Program:

 - [Tom Duncalf](http://blog.jenkster.com/):
    [Functional Programming Concepts](#kris-jenkins--what-is-functional-programming)
 - Ben Ford ([@ccrisccris](https://twitter.com/ccrisccris)):
    [Various Ways of Using Haskell](#cristiano-calcagno-functional-programming-at-facebook)

## Tom Duncalf: Functional Programming Concepts

![Tom Duncalf on stage](/notes/images/2016-02-09-ldn-functionals-5/DSCF4110.JPG)

Professor Frisby's Mostly Adequate Guide to Functional Programming -introduction to func programming in js


pure function is a function that given the same input will always return same output
plus no observable side effects

type signatures



Hindley- Milner type signatures

// stringLength :: String -> Number


First class functions

treated like any other data type
can be passed as argument, stored in var, array etc,
they are only called when invoked with()

curried functions


can be called with fewer arguments than it expects
if called with fewer args will return a "partially appplied" function  that takes the remaining arguments
allow us to make new domain specific functions from generic one

Composition

-
f and g are function , x is the value being piped through them

function(f, g) {
return function (x) {
return f(g(x))
}}

doesn't mention data we working on
good indication how functional code is

handling errors??

Functors

is a type that implements map and obeys some laws

example:e
Maybe functor
for handling null responses
IO
Task


Monads

(nested functors lead to uncomfortable code)

are functors with join and ..
chain function (flat_map)



## Ben Ford: Various Ways of Using Haskell

![Ben Ford on stage](/notes/images/2016-02-09-ldn-functionals-5/DSCF4111.JPG)


HAskel

Miyamoto Musashi



zygohistomorphic prepromorphisms

Combining Structures is the essence of Haskell
Monoid

The strategist makes small things into big things.

Folds


Practical recursion schemes - Jared Tobin

think lightly of yourself and deeply of the world


---


### Date:

2016-02-23 18:30

### Location:

Skills Matter | CodeNode, 10 South Place, London, EC2M 7EB

### Met:

[Anna](https://twitter.com/lithinn), [Roman](https://twitter.com/romanschejbal)





