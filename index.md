# So you want to run a transport code for space radiation?
## What is radiation transport?
[Learn here](./transport.html)

## How are Monte Carlo methods applied to radiation transport?
[Learn here](./montecarlo/explainer.html)

### What Monte Carlo radiation transport codes are available?
[See here](./montecarlo/codes.html)

## How are deterministic methods applied to radiation transport?
[Learn here](./deterministic/explainer.html)

### What deterministic radiation transport codes are available?
[See here](./deterministic/codes.html)

## What jargon should you know?
Automated computation of radiation transport evolved in the 1940s and 50s, so some of the terminology reflects that period rather than modern usage.

| Jargon | Synonym | Explanation |
| ------ | ------- | ----------- |
| card | input data/file | defines the setup of the transport problem (*e.g.* materials card, geometry card, (radiation) source card)
| code | program | the computer program that transports the radiation |
| filter | region | the region of interest |
| (input) deck | | the overall collection of input data and files that define the transport problem |
| score | statistic | the event, function, or statistic of interest |
| tally | output data/file | final output data based on filter and score from a (set of) particle(s) |
| transport | movement | the process of moving the radiation particles (or quanta) through a specified medium |

A **tally** may be the dose in water from neutrons behind a shield material.
A **filter** would be the volume of that water region.
A **score** would be the energy deposited (dose).

# All resources
[Click for a helpful list of resources that doesn't fit neatly into siloed categories](./collated.html)
