---
title: Team Block Diagram
---

## Introduction

Team 209 **_Smart Door Sensor System_** block diagram.
A block schematic of how the individual sub-systems are expected to be connected to individual components and between each other to create a working device.

## Images


<img width="4116" height="794" alt="Team 209 drawio" src="https://github.com/user-attachments/assets/ac8dc5e2-99de-4a83-b6ba-d743f0f356f1" />
**Figure 1:** Initial Block Diagram of Member Components.

## Decision Making Process
The door sensor system block diagram reflects how the team structured the processes that run between the sub-systems and components, after reviewing each sub-system against the product and course requirements. 
<br> After selecting the components in each sub-system, we designed how the serial communication is expected to flow between them, and which of the systems needs to send an output and receive and input from the others. 
<br>We hence settled on a central node at the ultrasonic sensor which only sends out values of the distance, and interconnected branches which share information and logic between themselves.

## Product Requirements
The Block Diagram fulfils the basic functionality needs of the Smart Door Sensor. It has components and systems capable of both sensing and actuation that adapt communication between boards to ensure security.


## Team Connections
**Table 1: Connector between Bryce and Andrew**

| Pin |	From	| To	| Type | Description|
|-----|------|------|------|-------|
| 1 | - | - | - | not used |
| 2 | - | - | - | not used |
| 3 | - | - | - | not used |
| 4 | - | - | - | not used |
| 5 | Bryce (RF5) | Andrew (RF6) | 0V / 5V Digital | Door is Closed / Door is Open |
| 6 | - | - | - | not used |
| 7 | - | - | - | not used |
| 8 | Ground | Ground | Ground | Ground |


**Table 2: Connector between Bryce and Dylan**

| Pin |	From	| To	| Type | Description|
|-----|------|------|------|-------|
| 1 | - | - | - | not used |
| 2 | - | - | - | not used |
| 3 | - | - | - | not used |
| 4 | - | - | - | not used |
| 5 | Bryce (RF5) | Dylan (RF6) | 0V / 5V Digital | Door is Closed / Door is Open |
| 6 | - | - | - | not used |
| 7 | - | - | - | not used |
| 8 | Ground | Ground | Ground | Ground |

**Table 3: Connector between Mathew and Dylan**

| Pin |	From	| To	| Type | Description|
|-----|------|------|------|-------|
| 1 | - | - | - | not used |
| 2 | Mathew (RB2) | Dylan (RF5) | 0V / 5V Digital | Unlock Sequence |
| 3 | - | - | - | not used |
| 4 | - | - | - | not used |
| 5 | - | - | - | not used |
| 6 | - | - | - | not used |
| 7 | - | - | - | not used |
| 8 | Ground | Ground | Ground | Ground |

**Table 4: Connector between Andrew and Dylan**

| Pin |	From	| To	| Type | Description|
|-----|------|------|------|-------|
| 1 | - | - | - | not used |
| 2 | - | - | - | not used |
| 3 | - | - | - | not used |
| 4 | Andrew (RD5) | Dylan (RF7) | 0V / 5V Digital | Alarm / Lock Toggle Switch |
| 5 | - | - | - | not used |
| 6 | - | - | - | not used |
| 7 | - | - | - | not used |
| 8 | Ground | Ground | Ground | Ground |


##  Top 5 changes to our software design
1. We are outputing a digital signal instead of an analog signal to determine that our door is open or closed. We had it outputing an analog signal but that would have been confusing to each other and there was no point. Instead we are sharing a signal that tells if the door is open or closed.
2. We removed our timer for the alarm system, as it did not work. It just paused the entire system waiting to turn on the alarm, so it was changed to be an instant activation.
3. We changed our motor idea, as we were planning on using an encoder to track where the lock was and if the door was locked or unlocked. Instead we got rid of that because it got very confusing to try and code and wire.
4. Our unlocking sequence was changed from a big combination to a few button input. It was too complicated to make a big code with the shift register so we simplified the design. 
5. The overall software changed to make everything work better. We were sending a mix of signals that did not make sense anc checking for things that did not work. So we changed what we were outputing and made it more understandable.



