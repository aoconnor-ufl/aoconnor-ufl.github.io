---
title: Monte Carlo methods
---

# A brief explanation
![animated Monte Carlo calcuation of pi](https://upload.wikimedia.org/wikipedia/commons/8/84/Pi_30K.gif)[^1]

+ Thought experiment: throw a dart at a circle that is embedded within a square
+ Ratio of darts landing within circle to darts landing outside of circle approaches π
+ May take many thousands or even millions of trials to reach appropriate confidence level
+ “brute force” using inferential statistics from a sample, not deterministic


[^1]:animation by [nicoguaro](https://commons.wikimedia.org/wiki/File:Pi_30K.gif) under [CC BY 3.0](https://creativecommons.org/licenses/by/3.0/deed.en)

# Application to radiation transport
![image](https://user-images.githubusercontent.com/78624429/152051534-89e0096e-26d6-4071-9087-c252c8e6ade5.png)

+ Apply Monte Carlo methods to random walk: now one can simulate a particle of radiation moving through a medium and derive statistics
+ Requires tracking each particle: location, energy, interaction probability,etc.
  - Also must track any secondary radiation generated during primary particle interactions and so on
+ Complexity of individual-level tracking the history of (potentially) millions of particles necessitates a computational approach

# Resources that explain the Monte Carlo technique and/or its application to radiation transport

## Videos
### MIT 6.0002 -- Lecture 6: Monte Carlo simulation
YouTube link: <https://youtu.be/OgO1gpXSUzU>  *closed captioning available*

Slides: <https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-0002-introduction-to-computational-thinking-and-data-science-fall-2016/lecture-slides-and-files/MIT6_0002F16_lec6.pdf>

Course page: <http://ocw.mit.edu/6-0002F16>
### Writing a Monte Carlo Radiation Transport Code
Don't waste your time reinventing the wheel like this, but it may be helpful to understand the innner workings of such codes.

Link: <https://www.youtube.com/watch?v=nVvFQ0e8J8g>

## Websites
### UIUC MSTE
Contains an interactive, online applet demonstrating Buffon's Needle thought-experiment.
Demonstrates 1) regression to the mean: as the number of trials increases, the observed value will approach the expected value and 2) inferential statistics: provided a sufficient sample of a population, the population statistics may be inferred from the sample.

Link: <https://mste.illinois.edu/activity/buffon/>
### Scratchapixel
Though written for computer gaphics, this is also a great explainer with excellent visuals of Monte Carlo operation and techniques

Link: <https://www.scratchapixel.com/lessons/mathematics-physics-for-computer-graphics/monte-carlo-methods-in-practice/>
