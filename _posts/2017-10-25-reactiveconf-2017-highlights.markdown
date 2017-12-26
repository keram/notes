---
layout: post
title:  Highlights from ReactiveConf 2017
date:   2017-12-27 14:00:00 +0000
categories: conference
---
[![ReactiveConf banner](/notes/images/2017-10-25-reactiveconf-2017-highlights/preview/reactive.jpg)](/notes/images/2017-10-25-reactiveconf-2017-highlights/reactive.jpg)

[ReactiveConf](https://reactiveconf.com/) a conference of modern trends in web development, which brings the world top renowned speakers on such topics to Slovakia. It was the third year of the conference.

This year I attended the conference thanks to the generosity of friend [Johnny](http://mathalope.co.uk/) who for my luck couldn't go.

### Jonas

I flew to Slovakia one day in advance and had a chance stay overnight with friend, Slovak sound artist and craftsman [Jonas Gruska](https://lom.audio/artists/jonas-gruska/). His sound experiments, field recordings and instruments are well known (His latest album [Spevy](https://lom.audio/releases/jonas-gruska-spevy/) got also mentioned in the latest release of Wire magazine.)

[![Jonas Gruska and Wire magazine](/notes/images/2017-10-25-reactiveconf-2017-highlights/preview/jonas_wire.jpg)](/notes/images/2017-10-25-reactiveconf-2017-highlights/jonas_wire.jpg)

Good job! And You should definitely listen to some of his recordings released for example on [Bandcamp - Luky](https://jonasgruska.bandcamp.com/album/l-ky).
We eat pizza, played Go and listen to some pieces from his music collection.<br/>
The conference couldn't start better.
<br/>
<br/>

### [David Nolen: Out of the Tarpit, Revisited](https://www.youtube.com/watch?v=7y1phdZkLw4)

Wednesday morning, first speaker on stage [David Nolen](https://twitter.com/swannodette) shared ideas from Ben Moseley and Peter Marks paper - Out of the Tar Pit (2006), advocated for a simplicity and shared examples of use of [Datomic database](http://www.datomic.com/).

> When considered next to testing and reasoning, simplicity
is more important than either. Given a stark choice between investment
in testing and investment in simplicity, the latter may often be the better
choice because it will facilitate all future attempts to understand the system attempts of any kind.
>
> -- <cite>[Out of the Tar Pit - Ben Moseley, Peter Marks (2006)](http://curtclifton.net/papers/MoseleyMarks06a.pdf)</cite>

But I had also my personal reasons to be excited about the second year appearance of David at ReactiveConf besides of his talk. We had some business to do and a picture of two of us was captured and [shared by conference organisers](https://twitter.com/ReactiveConf/status/925080643024891904). :D

[![David Nolen, Jared Forsyth, me and Go match](/notes/images/2017-10-25-reactiveconf-2017-highlights/preview/david_go.jpg)](/notes/images/2017-10-25-reactiveconf-2017-highlights/david_go.jpg)

<br/>
<br/>

### [RON: Replicated Object Notation - Victor Grishchenko](https://www.youtube.com/watch?v=0Xx9kkTMi10)

The second technical talk to mention was Victor Grischenko's presentation where he made good arguments against overuse of JSON as an exchange format between nowadays applications.

Some of his arguments were:

- JSON is well readable by humans but not so as well understandable by computers
- is bloated
- weak (missing UUID, versioning..)

#### Alternative? [Swarm Replicated Object Notation](https://github.com/gritzko/swarm-ron)

> Distributed data serialization format.
Implicitly, formats like XML or JSON assume a lump of state being delivered from a server to a client -- once and in one piece.
RON aims to synchronize replicas by delivering a stream of changes -- continuously and incrementally.
With RON, even an object's state is seen as a batch of compacted changes, with more changes coming.
>


<br/>
<br/>

### [Secrets of the Glimmer VM - Tom Dale](https://www.youtube.com/watch?v=nXCSloXZ-wc)
[![Glimmer](/notes/images/2017-10-25-reactiveconf-2017-highlights/preview/glimmer.jpg)](/notes/images/2017-10-25-reactiveconf-2017-highlights/glimmer.jpg)

- Extracted from Ember as indepedent project, [Glimmer](https://glimmerjs.com/
) is a flexible, low-level rendering pipeline for building a "live" DOM from Handlebars templates that can subsequently be updated cheaply when data changes.

- Build in TypeScript, compiling to bytecode.

- [The Glimmer VM: Boots Fast and Stays Fast](http://yehudakatz.com/2017/04/05/the-glimmer-vm-boots-fast-and-stays-fast/) - blogpost by Yehuda Katz


### Ethereum Meetup at [Progressbar](https://www.progressbar.sk)

Thursday evening meand unexpected adventure, when the driver of the last bus (and connection) to my hometown, decided not to take any more passengers and I found myself standing at the bus station with free evening and with no particular plans for the night. Fortunately, the situation had happy end thanks to Matej and Ivanka and also managed attended very interesting meetup at local hackerspace Progressbar about cryptocurrencies and investments.

### Friday Workshops at FIT

On Friday the conference moved to a new location for a day full of workshops, discussions and screenings.
I attended a workshop on [Reason language](https://reasonml.github.io/) which together with talk day before ([Reason: JavaScript-flavored OCaml - Jared Forsyth](https://www.youtube.com/watch?v=lN78ystnVw4)) give good reason why I can recommend to keep eye on this language.

[![Reason](/notes/images/2017-10-25-reactiveconf-2017-highlights/preview/reason.jpg)](/notes/images/2017-10-25-reactiveconf-2017-highlights/reason.jpg)

One may get lost so to summarise:

- *Caml* (originally an acronym for Categorical abstract machine language) is a multi-paradigm, general-purpose programming language which is a dialect of the ML programming language family.
Caml was developed in France at INRIA and EN.S

- *OCaml* (Objective Caml) - implementation of Caml

- *BuckleScript* - A backend for the OCaml compiler which emits JavaScript.

- *Reason* - an alternate syntax (interface) for OCaml that uses Bucklescript compiler backend to output JavaScript.

<br>
Surprise moment was when I met in one of the conference rooms my cousin whom I haven't seen for over five years so the
conference become also a place of the family gathering.
<br />

### Post Conference and After Party


But the day wasn't over and time between official conference end and after party I spent in local tea-house meeting another local Go friend.
The special twist of our game was brought by the presence of Pavol Lisy (1p) First Slovak professional of the game of Go and one of the top players in Europe!

Then came after party which prepared also some funny moments. As every attendee received tokens for free drinks I headed to the bar and my discussion with barman follows:

Me: *What can I get for a token?*

Barman: *Beer, Wine, Vodka, Whiskey*

With a smile, I asked: *Which of that is non-alcoholic?*

Barman: *None*

Me: *Can I get sparkling water instead?*

Barman: *No, for the token you can choose only from Beer, Wine, Vodka, Whiskey or buy other stuff with your own money..*

Me:

![Multi facepalms](/notes/images/2017-10-25-reactiveconf-2017-highlights/facepalm.jpg)

To solve the puzzle, I asked for wine and glass of tap water with it which I got without a problem. :D

With drink with my hand, I met and chat with some familiar faces from the conference and workshop.
The last funny moment of the conference happens when after chatting with pair Rebecca and Sean from Manchester about the life and work as we all came from the UK. Later that night we found that their conference ticket number was 20 and 21. Mine was 22 which can be considered as proof that nothing happens as a coincidence! :D


**That was my ReactiveConf 2017 and I would like to thank organisers, speakers who came, friends and family who made the time spent in Slovakia special and great.**
#### Thank you and hope to see you again in 2018!

<br/>

---


### Date:

2017-10-24 - 2017-10-30

### Location:

Bratislava, Slovakia

### Website:

[Reactive Conf 2017](https://reactiveconf.com/2017/)


### Met:

Laila, Juraj B., Wao, Palko, pht, Ivanka K. Aoik, Jan G., Milos, Zuzka M., Radka G., ?, ?, ? ...

