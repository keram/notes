---
layout: post
title:  "LDNWebPerf Special - Tim Kadlec & Ilya Grigorik"
date:   2016-02-13 19:00:00 +0000
categories: meetup
---

### Program:

 - Tim Kadlec ([@tkadlec](https://twitter.com/tkadlec)):
    [Mobile image processing](#tim-kadlec-mobile-image-processing)
 - Ilya Grigorik ([@igrigorik](https://twitter.com/igrigorik)):
    [Webperf API's to quantify and improve real world RAIL](#ilya-grigorik-webperf-apis-to-quantify-and-improve-real-world-rail)


## Tim Kadlec: Mobile image processing

[![Tim Kadlec on stage](/notes/images/2016-02-11-web-perf-meetup/preview/DSCF4092.JPG)](/notes/images/2016-02-11-web-perf-meetup/DSCF4092.JPG)

Images on the web affect network bandwidth consumption and
also a performance of the browser, device and battery life.
Big images have large(unnecessary) footprint on CPU, GPU (decoding) and memory (storing decoded data to display)

To improve web performance we can not only serve images in the actual size they are used
but also, use subsampling when possible (JPEG-s).

> **Chroma subsampling** is the practice of encoding images by implementing less resolution for chroma information than for luma information, taking advantage of the human visual system's lower acuity for color differences than for luminance.
> -- <cite>[Wikipedia](https://en.wikipedia.org/wiki/Chroma_subsampling)</cite>

Keypoints:

 - meta viewport is your friend
 - small breakpoints for large images
 - use downsampling 4:2:0 if you can
 - for websites serving a lot of images use heuristic algorithms to find a best downsampling ratio
  to ensure that resized and downsampled image will be inside of the boundaries of the expected image quality by users.


## Ilya Grigorik: Webperf API's to quantify and improve real world RAIL

[![Ilya Grigorik on stage](/notes/images/2016-02-11-web-perf-meetup/preview/DSCF4098.JPG)](/notes/images/2016-02-11-web-perf-meetup/DSCF4098.JPG)

### Correlation between weather and speed of application.

Anectodal story about finding the cause of bad performance
 of one application in a specific location on mobile devices.
Lesson learned: In hot weather, to prevent overheating, device decide run fans and reduce CPU frequency (slows down application).

**RuM techniques for RAIL**

[The RAIL Performance Model](https://developers.google.com/web/tools/chrome-devtools/profile/evaluate-performance/rail?hl=en)

RAIL (stands for Response, Animation, Idle, Load) is a user-centric performance model. Every web app has these four distinct aspects to its lifecycle, and performance fits into them in very different ways.

[Web performance timing specifications](https://siusin.github.io/perf-timing-primer/)

Timing performance API-s using buffers have disadvantages and can actually affect the performance..

[Performance Observer](https://w3c.github.io/performance-timeline/#the-performance-observer-interface)
to the rescue. (In Chrome Canary)

### Response

Chain of latencies between user input and web application response:

``Touch`` ->
``hardware latency`` ->
``Operation System latency`` ->
``Browser latency`` ->
``Application latency`` -> ``Response``

``event.timeStamp`` -
 OS provided value for input events, event creation time for all other events.
It exists for a long time but implementations differ across browsers.

``Passsive Event Listeners`` -
Javascript event callbacks which don't call ``.preventDefault()`` (allows smooth scrolling)

### Animation + Idle

[Intersection Observer](https://github.com/WICG/IntersectionObserver/blob/master/explainer.md)
- for checking if the element is in viewport!
  (Ready in Canary with enabled experimental features)

[Paul Lewis](https://twitter.com/aerotwist) master plan: Make things done in 8 milliseconds

[requestIdleCallback](https://developers.google.com/web/updates/2015/08/using-requestidlecallback?hl=en)
- We can leverage free time slots in 16ms for additional work.

### Load

``declarative preconnect`` - Initiating TCP connections in advance

``reactive preconnect``

``declarative preload``

``Save-Data header``

[Async CSS with preload "hack"](https://filamentgroup.github.io/loadCSS/test/preload.html):

{% highlight html %}
<link rel="preload" href="style.css" as="style" onload="this.rel='stylesheet'">
{% endhighlight %}

More reading:

- [Eliminating Roundtrips with Preconnect](https://www.igvita.com/2015/08/17/eliminating-roundtrips-with-preconnect/)
- [HTTP Client Hints](httpwg.org/http-extensions/client-hints.html)

---

### Website:

[LDNWebPerf Special - Tim Kadlec & Ilya Grigorik](http://www.meetup.com/London-Web-Performance-Group/events/228452974/)

### Date:

2016-02-11 19:00 - 22:00

### Location:

Marks &amp; Spence Office, Waterside House, 35 North Wharf Road, London W2 1NW

### Photos:

[![Audience on break](/notes/images/2016-02-11-web-perf-meetup/preview/DSCF4094.JPG)](/notes/images/2016-02-11-web-perf-meetup/DSCF4094.JPG))
[![Ilya Grigorik and Perry Dyball](/notes/images/2016-02-11-web-perf-meetup/preview/DSCF4096.JPG)](/notes/images/2016-02-11-web-perf-meetup/DSCF4096.JPG)

