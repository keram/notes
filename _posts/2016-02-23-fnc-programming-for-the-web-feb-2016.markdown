---
layout: post
title:  "Functional Programming for the Web - Februar 2016"
date:   2016-02-28 10:00:00 +0000
categories: meetup
---

### Program:

 - [Tom Duncalf](https://twitter.com/tomduncalf):
    [Functional Programming Concepts](#tom-duncalf-functional-programming-concepts)
 - [Ben Ford](https://twitter.com/boothead):
    [Various Ways of Using Haskell](#ben-ford-various-ways-of-using-haskell)


## Tom Duncalf: Functional Programming Concepts

[![Tom Duncalf on stage](/notes/images/2016-02-23-fnc-programming-for-the-web-feb-2016/preview/DSCF4157.JPG)](/notes/images/2016-02-23-fnc-programming-for-the-web-feb-2016/DSCF4157.JPG)

Recommended reading:
[Professor Frisby's Mostly Adequate Guide to Functional Programming](https://github.com/MostlyAdequate/mostly-adequate-guide)

**Pure function** is a function that given the same input will always return same output and has no observable side effects.

> **Hindley–Milner type system**
>
> In type theory and functional programming, Hindley–Milner (HM) (also known as Damas–Milner or Damas–Hindley–Milner) is a classical type system for the lambda calculus with parametric polymorphism, first described by J. Roger Hindley and later rediscovered by Robin Milner. Luis Damas contributed a close formal analysis and proof of the method in his PhD thesis.
>
> Among HM's more notable properties is completeness and its ability to deduce the most general type of a given program without the need of any type annotations or other hints supplied by the programmer. Algorithm W is a fast algorithm, performing type inference in almost linear time with respect to the size of the source, making it practically usable to type large programs.[note 1] HM is preferably used for functional languages. It was first implemented as part of the type system of the programming language ML. Since then, HM has been extended in various ways, most notably by constrained types as used in Haskell.
> -- <cite>[Wikipedia](https://en.wikipedia.org/wiki/Hindley%E2%80%93Milner_type_system)</cite>

**First class functions** are functions treated like any other data type:
can be passed as argument, stored in var, array etc. They are only called when invoked with()

**Curried functions** can be called with fewer arguments than it expects.
If called with fewer args will return a "partially appplied" function that takes the remaining arguments
allow us to make new domain specific functions from generic one.

**Composition**

``f`` and ``g`` are functions, ``x`` is the value being piped through, then:


{% highlight javascript %}
function(f, g) {
    return function (x) {
        return f(g(x));
    }
};
{% endhighlight %}

Functions which doesn't mention data we working on are
good indication how functional code is.


**Functors**

 - is a type that implements map and obeys some laws

 - Maybe functor: for handling null responses
 - IO
 - Task

**Monads** are functors with join and ..chain function (flat_map)

### [Presentation](https://cdn.rawgit.com/tomduncalf/talks/ae830942b664fa48c7d1253085706b5187d24c41/FPFundementals/index.html)


## Ben Ford: Various Ways of Using Haskell

[![Ben Ford on stage](/notes/images/2016-02-23-fnc-programming-for-the-web-feb-2016/preview/DSCF4160.JPG)](/notes/images/2016-02-23-fnc-programming-for-the-web-feb-2016/DSCF4160.JPG)

Combining Structures is the essence of Haskell.

 - [zygohistomorphic prepromorphisms](https://wiki.haskell.org/Zygohistomorphic_prepromorphisms)
 - [Practical recursion schemes - Jared Tobin](https://medium.com/@jaredtobin/practical-recursion-schemes-c10648ec1c29)

**Miyamoto Musashi**

> (c. 1584 – June 13, 1645), also known as Shinmen Takezō, Miyamoto Bennosuke or, by his Buddhist name, Niten Dōraku, was an expert Japanese swordsman and rōnin. Musashi, as he was often simply known, became renowned through stories of his excellent, and unique double bladed swordsmanship and undefeated record in his 60 duels. He was the founder of the Hyōhō Niten Ichi-ryū or Niten-ryū style of swordsmanship and in his final years authored the The Book of Five Rings, a book on strategy, tactics, and philosophy that is still studied today.
> -- <cite>[Wikipedia](https://en.wikipedia.org/wiki/Miyamoto_Musashi)</cite>

 - The strategist makes small things into big things.
 - Think lightly of yourself and deeply of the world.

---


### Date:

2016-02-23 18:30

### Location:

Skills Matter | CodeNode, 10 South Place, London, EC2M 7EB

### Met:

[Anna](https://twitter.com/lithinn), [Roman](https://twitter.com/romanschejbal)

### Photos:

[![](/notes/images/2016-02-23-fnc-programming-for-the-web-feb-2016/preview/DSCF4155.JPG)](/notes/images/2016-02-23-fnc-programming-for-the-web-feb-2016/DSCF4155.JPG)
[![](/notes/images/2016-02-23-fnc-programming-for-the-web-feb-2016/preview/DSCF4161.JPG)](/notes/images/2016-02-23-fnc-programming-for-the-web-feb-2016/DSCF4161.JPG)

### [Video](https://www.youtube.com/watch?v=xyqTHLOra_I)



