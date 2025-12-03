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

| Pin |	From	| To	| Type | Description|
|-----|------|------|------|-------|
| 5   | Bryce (RF5) | Andrew (RF5) | 0V / 5V Digital | Door is Closed / Door is Open |









