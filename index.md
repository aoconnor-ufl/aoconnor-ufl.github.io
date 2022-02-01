# So you want to run a transport code for space radiation?
n.b. this primer focuses on radiation in aerospace environments, so certain codes or topics (_e.g._ criticality) common to radionuclear simulations may be abridged or neglected

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

### Jargon example
> The *absorbed dose* in the **water tank** is ***10.7 Gy***.
+ ***Tally***: dose in water from neutrons behind a shield material
+ **Filter**: volume of that water region
+ *Score*: energy deposited (dose)


![tally-1](https://user-images.githubusercontent.com/78624429/152056666-e0407e1f-c786-4833-a78f-2a8a27d25e5c.svg)

Only the indicated portion of the gamma’s path through the water tank contributes to the tally.
![tally-2](https://user-images.githubusercontent.com/78624429/152056672-2df5e09b-d774-45f1-9bba-7ef43f838613.svg)

However, the code must track all other particles in case a delta ray (secondary radiation) crosses through water tank
![tally-3](https://user-images.githubusercontent.com/78624429/152056677-1ed2d261-95c3-499f-8561-faccd69b2ec7.svg)


# All resources
[Click for a helpful list of resources that doesn't fit neatly into siloed categories](./collated.html)
