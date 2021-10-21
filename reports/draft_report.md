# Traffic Models with Cellular Automata

## Abstract
An accurate simulation of traffic is very useful tool that serves endless purposes. Due to their nature, specifically their simplicity and versatility, celular automata are ideal candidates to use in modelling unrealistic vehicular behaviour. However, microscopic traffic models (usually designed as a series of differential equations) are more accurate in modeling regulated traffic flow, but are computationally much more expensive. In this report we implement an agent-based model of a highway driving simulation based on a model in Mitchell Resnick’s book, Turtles, Termites and Traffic Jams. This involved independently acting drivers driving on a simlated highway. Following this, we plan to apply anti-collision behaviours to the drivers to observe how they behave in chaotic situations (such as in reponse to an initial crash on the high way). In their report, Rodaro and Yeldan introduce a similar idea of using a stochastic cellular automata traffic model in which space is continuous, and also se a fuzzy system to handle uncertainites in decision making. This enables the simulation of different driver behaviours. We will not be replicating Rodaoro and Yeldan's exeriment, however thieir report serves as a guide to get us started.

## Related Papers
https://arxiv.org/pdf/physics/0509082.pdf

This paper explores TCA models and methods to use cellular automata models and mathematical notations to quantify real world units and simulate traffic flow. TCA models arise from the physics discipline of statistical mechanics to reproduce correct macroscopic behavior based on microscopic interactions. It dives into behavioral aspects of several TCA models, including single to multi lane networks. They conclude that with a concise overview of TCA models in multi-lane settings, a brake-light TCA model is the most promising. Though they state that these models are rapidly evolving further and further as we attempt to describe individual behaviors within a large scale road network.

https://arxiv.org/pdf/1302.0488.pdf?fbclid=IwAR0xm4DURepbl-D6eBnUAx677OVSQzO9nmJ_aw1pttb3FzLtI-rpXqqeS24

This paper explores a new method of simulating vehicular behavior and traffic modeling. Usually, one would choose to prioritize computational efficiency or realism when trying to model this behavior, but this research proposes a new class between these categories, combining efficiency from cellular automata models and accuracy of other microscopic models. This new traffic model would be based on continuous cellular automata. The conclusion came to an inconclusive analysis, but the report gave insight into the potentiality of a new way to simulate this behavior through continuous CA.

## Tools: [Agent Based Models](https://greenteapress.com/complexity2/html/thinkcomplexity2010.html)
Agent based models are a tool that can  be used to model independently acting entities such as people or, in this case, drivers. For our purposes, we will place each agent in a location on our highway and have them interact with only information from neighboring drivers; they have no knowledge of the system as a whole. We include a random characteristic to our drivers to give each driver unique characteristics.

## Experiments and their Replications
### Experiments
We replicated the Highway Traffic Model in Mitchell Resnick’s book, "Turtles, Termites and Traffic Jams" with guidance from Chapter 10 in "Think Complexity 2e
by Allen B Downey. 
### Variations
We plan to assign independent anti-collision behaviours to each driver, and then measure their behaviour and the number of collisions that occur with different numbers of cars on the highway.
A stretch-goal for our variations is to implement a multi-lane model and enable the drivers to swerve between lanes as a defensive maneuver and measure the number of collisions that occur in this set up. 
## Sample Results of Replicated Model:

![image](https://user-images.githubusercontent.com/42980963/138190280-cc4c74ad-109e-4712-9884-3bd6d98c21b9.png)

This model shows a series of square cars on a circular highway. The red triangles appear adjacent to any two cars that collide (by their shapes overlapping on the windwo space). 
## Predicted Results of Extension- Sketch
![image](https://user-images.githubusercontent.com/42980963/138191528-2a3c2864-62fd-455a-901b-380f0f428f11.png)
![image](https://user-images.githubusercontent.com/42980963/138191535-b6f7da17-3062-49d6-a368-51fb0ffea8b5.png)


![image](https://user-images.githubusercontent.com/42980963/138197530-b2182248-0f1c-4bd2-9565-be3576ed1876.png)


## Interpretation of Result
This model shows a multi-lane implementation of our traffic model-- what we expect to see when we implement our extension, along with some obstacles (such as road barricades) that hinder the traffic flow causing cars to switch lanes (ie turn from circles into squares). Here, again, the cars are considered to have collided when their shapes overlap. The collisions are marked here by the red x's. We will measure the relationship between the number of cars in the model and the number of collisions that ocur in a period  time given independent agents for this mode. We expect higher amounts of randomness in the system to cause more collisions when more cars are present. 
This is represented in the graph.

## Areas of Concern
One major area of concern is that this model does not have any steps for validation.
We are also unsure how to go about setting up the arrangement for multi-lanes, and the merging of vehicles between them. This may be a challenge we leave as a stretch goal. 

## Next Steps
### Individual Goals
#### Mahima
Implement of anti-colliding drivers
#### Jason
