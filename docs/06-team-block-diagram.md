---
title: Team Block Diagram
---

## Introduction

Team 209 **_Door Sensor System_** block diagram.
A block schematic of how the individual sub-systems are expected to be connected to individual components and between each other to create a working device.

## Images

![Team 209 Block Diagram](https://github.com/user-attachments/assets/2a28f3db-b05c-4d11-b9c8-1d77bbe881f2)
**Figure 1:** Initial Block Diagram of Member Components.

## Decision Making Process
The door sensor system block diagram reflects how the team structured the processes that run between the sub-systems and components, after reviewing each sub-system against the product and course requirements. After selecting the components in each sub-system, we designed how the serial communication is expected to flow between them, and which of the systems needs to send an output and receive and input from the others. We hence settled on a central node at the ultrasonic sensor which only sends out values of the distance, and interconnected branches which share information and logic between themselves.

## Product Requirements
The Block Diagram fulfils the basic functionality needs of the Smart Door Sensor. It has components and systems capable of both sensing and actuation that adapt communication between boards to ensure security.
