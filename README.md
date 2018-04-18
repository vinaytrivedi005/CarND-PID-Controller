# PID Controller

### Effect of Proportional component(P):

Proportional component controls how fast Controller reacts to current error. Increasong proportional component will result, in this project, for car to turn sharply towards the center and oscilate more and vice versa.

### Effect of Derivative component(D):

Derivative component controls how strongly Proportional component will affect to current error. In other words, derivative component will control overshoot and help converge Controller to its desired result.

### Effect of Integral component(I):

Integral component helps controller to converge to its desired output even if there exist some system bias.

### Choosing Hyperparameters:

I used manual approach to tune hyper parameters.

First I tried to control oscilation of car to be as minimum as possible using Proportional component. After P component was good enough and Contoller was not improving any further, I tuned derivative component to stop oscillation and make system converge to desired output. After system was getting relatively stable but not absolutely stable in turns, I used Integral component to react to continuous larger error so that in turns, when sum of errors get larger, system reacts faster and also if there is any system bias, it can be overcame. 