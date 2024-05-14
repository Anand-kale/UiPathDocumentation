# UiPath State Machines

## Overview

State machines basically work with a finite number of states for it execution
it changes state if any other activity triggered that activity.

We see that concept in Theory of computation like finite state automata, infinite state automata.

How to implement a guess number using state machine
-
In UiPath 3 activity for creating a state machine
* Here we have **Final State**, **State**, **State Machine** activities in UiPath Studio.
![Activities](image_11.png)
* State Machine provides boilerplate or structure of state machines.
* State provides a simple state were we need to configure it according to our need.
* Final State provides where all processes get terminated
![Guess Number Robot](image_12.png)
* Initializing State
  - We assign any random number to variable
  - ![Init State](image_13.png)
* Guess Number State
  - Taking input from user of any number if that number match then change state to final state
  - If not, then call Guess number state
  - ![Guess Number State](image_14.png)
* Final Number
  - If all conditions are satisfied, then change the Final State.
  - ![Final State](image_15.png)


