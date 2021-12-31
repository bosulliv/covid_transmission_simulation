# COVID Virus Transmission Simulation

## Overview

The intent of this repo is to build a naive simulation of covid transmission
by specifically modelling nudge and peer pressure. Where nudges are direct
urgent messages from the government and/or the media. And peer pressure
specifically changes the likelihood of the desire to wear a mask in certain
situations.

This modelling will be hopelessly biased - I am just going to model my
interactions. So I do not expect this to roll-up into a UK predictive model. The
intent is to see what it takes to produce a model that converges: My hunch is
that this is very hard, and as you add variables it will tend to diverge
strongly. 

Why? Because it is now the only way to understand the dynamics of infection.
When the pandemic started and we were all vulnerable - it was scarily easy to
model with a simple Gamma function. But in year two, we are no longer as
vulnerable, and we change our behaviour based on our perception of risk.

## Key Ideas

The model will be made up of interactions. Interactions are events with other
people. The number and type of interactions are governed by risk, which can be
strongly changed by a nudge. And once in an interaction, the key variable is
propensity to wear a mask. This changes the risk of being infected should an
infectious person be present. There are also important interactions preceded by
widespread lateral flow tests, which change the incidence of infectious
individuals.

nudge -> influences frequency and type of interactions

interaction has a risk dependent on ->
density
proximity events
number of people
pre-test
mask-wear
peer pressure

I can then make all of these variables random variables with different
probability distributions. And then I can experiment with the values that make
the greatest impact on transmission.

