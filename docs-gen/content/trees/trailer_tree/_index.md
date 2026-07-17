---
title: Trailer tree
weight: 20
chapter: true
---

# The trailer tree
Two variants of trailer trees are available.\
One variant where a scenario with a truck pulling multiple trailers is represented by one tree containing all the trailers,
with each trailer on a separate branch of the tree.\
The other variant where the same scenario is represented by multiple trees, one tree per trailer.

## Trailer types
The vspec trailer tree is a super tree that contains signal definitions for a large set of different trailer types.
The vspecPreprocessor can then be used to configure it for a specific trailer type and model.

An initial list of trailer types that are planned to be supported by the vspec files are:
* SEMI_TRAILER
* CENTER_AXLE_TRAILER
* FULL_TRAILER
* CONVERTER_DOLLY
* LINK_TRAILER
* TOWING_SEMI_TRAILER
* TOWING_CENTRE_AXLE_TRAILER
* TOWING_FULL_TRAILER

Further trailer types are planned to be added to the list.
