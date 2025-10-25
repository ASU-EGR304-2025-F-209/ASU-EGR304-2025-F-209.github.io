---
title: Software Proposal
---

## Introduction

The door controller firmware operates as a finite-state machine (FSM) which runs inside a cooperative main loop that follows this sequence: Read Inputs → Update State → Set Outputs. The system starts its operation by setting hardware registers to their initial values and clearing all software variables and establishing communication links between MCUs through UART and I²C interfaces and then it enters State 001 (Closed). The system checks debounced sensor inputs from magnetic reed/limit switches and distance/UART and current/thermal flags and user override buttons during each cycle. The Update State routine checks transition predicates after which Set Outputs determines motor driver and indicator output values based on the current state. The design structure produces reliable operation while making testing easier and blocking any potential output irregularities.

## Research Question

* Bullet Point 1
* Bullet Point 2
* Bullet Point 3

## Images

![image caption](StateMachineDiagram.png)

## Results

1. Numbered Point 1
1. Numbered Point 2
1. Numbered Point 3

## Conclusions and Future Work

## External Links

[example link to idealab](https://idealab.asu.edu)


## Results

1. Numbered Point 1
1. Numbered Point 2
1. Numbered Point 3

## Conclusions and Future Work

## External Links

[example link to idealab](https://idealab.asu.edu)


## References


