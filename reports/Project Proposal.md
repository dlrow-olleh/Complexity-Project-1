# Modelling Traffic with Cellular Automata

###### by Mahima Beltur and Jason Sol

## Abstract

An accurate simulation of traffic is very useful tool that serves endless purposes. Due to their nature, specifically their simplicity and versatility, celular automata are ideal candidates to use in modelling unrealistic vehicular behaviour. However, microscopic traffic models (usually designed as a series of differential equations) are more accurate in modeling regulated traffic flow, but are computationally much more expensive. The report we are following for this project takes a combined approach. They introduced the idea of using a stochastic cellular automata traffic model in which space is continuous, and also se a fuzzy system to handle uncertainites in decision making. This enables the simulation of different driver behaviours. For this project, we will first mimic Rodaro and Yeldan's model using the same stochastic and fuzzy models, and then attempt to see how well this model holds when various constraints are involved in driving such as: road barricades, or the need to change lanes.


## Annotated Bibliography
https://arxiv.org/pdf/physics/0509082.pdf


This paper explores TCA models and methods to use cellular automata models and mathematical notations to quantify real world units and simulate traffic flow. TCA models arise from the physics discipline of statistical mechanics to reproduce correct macroscopic behavior based on microscopic interactions. It dives into behavioral aspects of several TCA models, including single to multi lane networks. They conclude that with a concise overview of TCA models in multi-lane settings, a brake-light TCA model is the most promising. Though they state that these models are rapidly evolving further and further as we attempt to describe individual behaviors within a large scale road network. 
 

https://arxiv.org/pdf/1302.0488.pdf?fbclid=IwAR0xm4DURepbl-D6eBnUAx677OVSQzO9nmJ_aw1pttb3FzLtI-rpXqqeS24


This paper explores a new method of simulating vehicular behavior and traffic modeling. Usually, one would choose to prioritize computational efficiency or realism when trying to model this behavior, but this research proposes a new class between these categories, combining efficiency from cellular automata models and accuracy of other microscopic models. This new traffic model would be based on continuous cellular automata. The conclusion came to an inconclusive analysis, but the report gave insight into the potentiality of a new way to simulate this behavior through continuous CA. 


## Experiments and their Replications

### Experiments

*  One we intend to replicate is Rodaro and Yeldan's schocastic model of traffic.
*  Another potential area for replication is Maerivoet and Bart De Moor's model of city traffic.

### Variations

* We decided to adopt one of the recommended variations from 'A multi-lane traffic simulation model via continuous cellular automata' by Rodaro and Yeldan. They recommend, as an extension, that fuzzy logic-based systems to be used to explore these traffic systems. One variation to implement would be to translate the stochastic model from Rodaro and Yeldan's report into a fuzzy-logic system using 'Cellular Automata Models of Road Traffic' by Maerivoet and De Moor as a guide.
* A second variation would be to extend the rules of these models to reflect lane-changing behaviours, or to add barricades in the car's path to see how the flow may change.
* Another potential variation we could try is to incorporate real-life data into the model by Rodaro and Yeldan and attempt to validate them since they have not taken this step as of yet.

## Predicted Results- Sketch
Title: Traffic Phases in single vs multi-lane traffic
![image](https://user-images.githubusercontent.com/42980963/135946993-f8c8e22a-2c8c-41ae-a00c-ccbd764ee847.png)

## Interpretation of Result

By assessing the slop of the graph, we will be able to estimate the flow rate. A higher, positive slope will indiciate free-flowing traffic, while a low slope will indicicate syncronized movement. Negative slopes will represent a jam.

## Areas of Concern

In Maerivoet and De Moor's, while they provide many images of results from their automata, they don't actually let us in to how these model's were set up. Specifically, not in a easy to replicate way with pseudocode. However, they do provide a lengthy explanation for the derivation of their processes, so code can be derived from there.

Neither of the reports have validated their models in any significant way. Both of them run the simulation on model vehicles, and have not incorporated real-life traffic data into their systems. 

There does not seem to be a high amount of traffic data readily availalble to use. While there are many available to purchase, the datasets seem to cost thousands of dollars per month- which, in our situation, is unreasonable.

## Next Steps

### First Week Individual Goals

* Mahima
  * Understand theory behind stochastic CAs
  * Implement the single-lane traffic model from pseudocode
* Jason
  * Focus on understanding implementation understanding of how to turn it fuzzy
  * Implement the Multi-lane traffic model from pseudocode

### First Week Team Goals
Our first week goals are to get a thorough understanding of the literature we are using-- specifically the report by Rodaro and Yeldan. We will also attempt to implement the pseudo code provided in their report.
